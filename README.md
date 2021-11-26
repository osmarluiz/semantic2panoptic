# semantic2panoptic

The Semantic2Panoptic Jupyter Notebook shows an example of how to obtain panoptic segmentation results using semantic segmentation models with a simple data modification.

What you need to obtain these results:

- Identify what are the stuff and thing classes on your dataset.
- Create buffers (borders) on the "thing" classes that may merge, e.g., cars, houses. Not all objects will have this problem. For example, swimming pools are sufficiently apart from each other. Each buffer must contain a new value. This will ease the process of model evaluation.
- Select a semantic segmentation model. In this example, we used the Semantic Segmentation Models repository which contains many architectures and backbones.
- We suggest giving weights to each class since it might be very imbalanced. In the Jupyter Notebook we show how to do this.
- Use the function semantic2panoptic to obtain the panoptic results
