# Udacity Data Scientist Capstone Project ML Dog Breed Recognition Project
This contains the code for the final capstone project in the Udacity Data Scientist Nano Degree. In this project an image classification model is build and trained to classify images of dogs into 133 possible dog breed categories. Furthermore a blog post with the findings has been written to present my work.

While this particular project is mostly of academic nature, image classification has a wide variety of uses ranging from national security over automating everyday tasks.

# Libraries used
**sklearn**: provides machine learning tools

**keras**: a high-level neural networks API for building and training deep learning models

**numpy**: provides scientific computing tools

**glob**: allows for easy matching of directory paths with wildcard characters

**random**: generates random numbers

**cv2**: computer vision library for image processing

**matplotlib**: library for plotting data and creating graphs.

**tqdm**: progress bar library for displaying progress of long-running tasks

**PIL**: python Imaging Library for creating, manipulating, and transforming images

**extract_bottleneck_features**: function for extracting bottleneck features from pre-trained models

# Files
* \bottleneck_features
  * DogResnet50Data.npz: Resnet50 bottleneck features
  * DogVGG16Data.npz: VGG16 bottleneck features
* \images
  * images needed in the jupyter notebook
* dog_app.ipynb: jupyter notebook containing all code

# Project Components
The final model uses transfer learning obtaining it's features from a provided ResNet50 model. These are then pooled and passed into 133 nodes (one per dog breed) to determine the most likely breed. This works well as the dataset is fairly small with few features to detect.


# Instructions
Follow the instructions in the jupyter notebook to build and run the code step by step.


# Licensing, Authors and Acknowledgements
The framework for this project was provided by Udacity as part of their Data Scientist Nano Degree
