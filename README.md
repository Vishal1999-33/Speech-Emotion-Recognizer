# Python Project on Speech Emotion Recognition.
The main objective of this project is to build a model to recognize emotion from speech using the librosa and sklearn libraries and the RAVDESS dataset.


Speech Emotion Recognition is a process in order to recognize human emotion and affective states from speech.Voice often reflects underlying emotion through tone and pitch.
Librosa, a python library used for analyzing audio and music, is used for this recognition. It has a flatter package layout, standardizes interfaces and names, backwards compatibility, modular functions, and readable code. Soundfile is used to read and write sound files. It is an audio library based on libsndfile, CFFI and NumPy.


In order to install librosa and soundfile, following are the commands with anaconda prompt:-

  Librosa:-
  
     conda install -c conda-forge librosa
     conda install -c conda-forge/label/gcc7 librosa
     conda install -c conda-forge/label/cf201901 librosa
     
  Soundfile:-
  
     conda install -c conda-forge pysoundfile
     conda install -c conda-forge/label/gcc7 pysoundfile
     conda install -c conda-forge/label/cf201901 pysoundfile


We will load the data, extract features from it, then split the dataset into training and testing sets. Then, we’ll initialize an MLPClassifier and train the model.
MLPClassifier implements a multi-layer perceptron (MLP) algorithm that trains using Backpropagation.A Multi-layer Perceptron (MLP) is a supervised learning algorithm that learns a function f(.):R^m-->R^o by training on a dataset, where m is the number of dimensions for input and  o is the number of dimensions for output. Given a set of features X and a target y, it can learn a non-linear function approximator for either classification or regression. It is different from logistic regression, in that between the input and the output layer, there can be one or more non-linear layers, called hidden layers. Figure shows a one hidden layer MLP with scalar output.


![multilayerperceptron_network](https://user-images.githubusercontent.com/54469035/68450930-be15fb80-0212-11ea-8e3b-1a75e3981704.png)

The leftmost layer, known as the input layer, consists of a set of neurons representing the input features. Each neuron in the hidden layer transforms the values from the previous layer with a weighted linear summation (w*x), followed by a non-linear activation function  g(.):R-->R - like the hyperbolic tan function. The output layer receives the values from the last hidden layer and transforms them into output values.

The module contains the public attributes coefs_ and intercepts_. coefs_ is a list of weight matrices, where weight matrix at index i represents the weights between layer i and (i+1) layer . intercepts_ is a list of bias vectors, where the vector at index i represents the bias values added to layer (i+1).

Ravdess Dataset is the Ryerson Audio-Visual Database of Emotional Speech. It consists of data related to 24 actors each having 60 individual different kind of speech.This dataset looks like this:-


![dataset-simple-python-project](https://user-images.githubusercontent.com/54469035/68451694-c15eb680-0215-11ea-8d80-152e65fc593b.png)



