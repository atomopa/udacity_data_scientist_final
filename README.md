# Udacity Data Scientist Capstone Project ML Dog Breed Recognition Project
This contains the code for the final capstone project in the Udacity Data Scientist Nano Degree. In this project an image classification model is build and trained to classify images of dogs into 133 possible dog breed categories. Furthermore a blog post with the findings has been written to present my work.

While this particular project is mostly of academic nature, image classification has a wide variety of uses ranging from national security over automating everyday tasks.

For a more detailed overview, this is the official project motivation provided by Udacity (see Jupyter notebook).

 ### Why We're Here 

In this notebook, you will make the first steps towards developing an algorithm that could be used as part of a mobile or web app.  At the end of this project, your code will accept any user-supplied image as input.  If a dog is detected in the image, it will provide an estimate of the dog's breed.  If a human is detected, it will provide an estimate of the dog breed that is most resembling.  The image below displays potential sample output of your finished project (... but we expect that each student's algorithm will behave differently!). 

![Sample Dog Output](images/sample_dog_output.png)

In this real-world setting, you will need to piece together a series of models to perform different tasks; for instance, the algorithm that detects humans in an image will be different from the CNN that infers dog breed.  There are many points of possible failure, and no perfect algorithm exists.  Your imperfect solution will nonetheless create a fun user experience!

### The Road Ahead

We break the notebook into separate steps.  Feel free to use the links below to navigate the notebook.

* [Step 0](#step0): Import Datasets
* [Step 1](#step1): Detect Humans
* [Step 2](#step2): Detect Dogs
* [Step 3](#step3): Create a CNN to Classify Dog Breeds (from Scratch)
* [Step 4](#step4): Use a CNN to Classify Dog Breeds (using Transfer Learning)
* [Step 5](#step5): Create a CNN to Classify Dog Breeds (using Transfer Learning)
* [Step 6](#step6): Write your Algorithm
* [Step 7](#step7): Test Your Algorithm



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
* \images
  * images needed in the jupyter notebook
* dog_app.ipynb: jupyter notebook containing all code

# Project Components
The final model uses transfer learning obtaining it's features from a provided ResNet50 model. These are then pooled and passed into 133 nodes (one per dog breed) to determine the most likely breed. This works well as the dataset is fairly small with few features to detect.


# Instructions
Follow the instructions in the jupyter notebook to build and run the code step by step.


# Licensing, Authors and Acknowledgements
The framework for this project was provided by Udacity as part of their Data Scientist Nano Degree
