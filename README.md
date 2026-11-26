# Image Map Annotation

**A single, standalone Jupyter notebook for annotating an image dataset interactively**, built on [jupyter-scatter](https://github.com/flekschas/jupyter-scatter) and [ipywidgets](https://github.com/jupyter-widgets/ipywidgets). It runs in JupyterLab, VS Code and Google Colab.

Use it when you have images and their embeddings (CLIP, DINOv2, ResNet or plain pixels) and want to:
1. label them for a classifier with as few labels as possible;
2. find out what an unlabeled collection contains.

What the notebook does:
1. Builds a 2D map of the embeddings, where similar images sit together.
2. Asks you to label a well-spread set of images by clicking, one per grid cell on the map.
3. Predicts labels for the rest, and points the next round at the images it is least sure about.