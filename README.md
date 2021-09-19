# Disaster-Management-Web-App

The following section gives a brief overview of the complete project from describing the
problem identified by and solutions provided by the literature review and the current
technology available.
The project focuses on disaster recognition/classification and damage evaluation in the data
provided. The data provided could be in the form of Images, Videos, or remote sensing data
like Satellite Images etc. The AI system provides user the functionality to identify disasters in
a certain multimedia file and the extent of damage through remote sensing data. In this project,
we have used Neural Networks to train the system to recognize different kinds of disasters form
regular everyday images and to estimate damage done through remote sensing data. Neural
networks are a class of machine learning algorithms used to model complex patterns in datasets
using multiple hidden layers and non-linear activation functions. A neural network takes an
input, passes it through multiple layers of hidden neurons (mini-functions with unique
coefficients that must be learned), and outputs a prediction representing the combined input of
all the neurons.
To create this project datasets, dataset is collected from multiple sources such as Kaggle
multiple AI blogs and data scraped from online image sources like google images, flicker etc.
and then the data is labelled.
After that data is pre-processed for example by bringing all image data into the same RGB
colour space and then reduced to the same size and then the resultant array is then normalized
which leads to better prediction accuracy. For the Disaster Evaluation model one more step is
performed that is to concatenate pre-disaster and post-disaster image.
After This multiple transfer learning techniques like VGG, XceptionNet, ResNet etc. are used
to train the machine learning model and the technique with the best results is used in the final
model. The model is then exported into an .HDF5 or .H5 file. Transfer learning is the reuse of
a pre-trained model on a new problem. It's currently very popular in deep learning because it
can train deep neural networks with comparatively little data. This is very useful in the data
science field since most real-world problems typically do not have millions of labelled data
points to train such complex models.
Models are analysed for performance of prediction. The proposed system has been trained with
several different models; however, the final system uses one based on the selected attributes,
which was an output of the classifier attribute evaluation from an ML tool. All ML models
developed were validated using evaluation criteria, i.e., Accuracy and F1-Score. These metrics
are used for summarising and assessing the quality of the ML model. To efficiently compare
the proposed model with other methods, we formed a sub-dataset which consist of 15% of the
original dataset. When used at production level, XceptionNet gives the best Accuracy & F1-
Score whereas theoretically DenseNet121 gives the best Accuracy & F1-Score. Since the best
model is the one which performs best for random images therefore XceptionNet turns out to be
the best model for our use-case. 
The web portal is made through web technologies like HTML5 and Streamlit for the front end
to make it more user friendly and interactive while using backend frame works like Flask to
power the server-side machinery in and running the ML model. The Web portal is deployed
using Microsoft Azure. The web portal provides user the functionality to input image or video
of a disaster and to get disaster class and extent of disaster damage as an output.
