<img src="core-ml.png" align="left" width="64"> 

# Awesome Core ML models [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

This repository has a collection of Open Source machine learning models which work with Apples **Core ML** standard.

Apple has published some of their own models. They can be downloaded [here](https://developer.apple.com/machine-learning/).
Those published models are: **SqueezeNet, Places205-GoogLeNet, ResNet50, Inception v3, VGG16** and will not be republished in this repository.

## Contributing
If you want your model added simply create a pull request with your repository and model added. In order to keep the quality of this repository high you have to conform to this project structure (taken from **@hollance**).

```
├── Convert
│   ├── coreml.py
│   ├── mobilenet_deploy.prototxt
│   └── synset_words.txt
├── MobileNet.mlmodel
```

There has to be a **Convert** directory with the Python script and additional data to reproduce this model on your own. If your model requires a huge amount of data please include a script which downloads those files. The **.mlmodel** file is optional because you'll have to push it onto this repository anyways.

```
├── MobileNetCoreML
│   ├── *.swift
├── MobileNetCoreML.xcodeproj
│   ├── project.pbxproj
│   └── project.xcworkspace
│       └── contents.xcworkspacedata
├── README.markdown
```

You also have to have an Xcode project where the user can test the model (sample data included would be nice).

## Models

### MobileNet
Model: [MobileNet.mlmodel](https://github.com/hollance/MobileNet-CoreML/raw/master/MobileNet.mlmodel)

Description: Object detection, finegrain classification, face attributes and large scale geo-localization

Author: [Matthijs Hollemans](https://github.com/hollance)

Reference: [MobileNets: Efficient Convolutional Neural Networks for Mobile Vision Applications](https://arxiv.org/abs/1704.04861v1)

Example: [MobileNet-CoreML](https://github.com/hollance/MobileNet-CoreML)

### MNIST
Model: [MNIST.mlmodel](https://github.com/ph1ps/MNIST-CoreML/raw/master/MNISTPrediction/MNIST.mlmodel)

Description: Handwritten digit classification

Author: [Philipp Gabriel](https://github.com/ph1ps)

Reference: [MNIST handwritten digit database](http://yann.lecun.com/exdb/mnist/)

Example: [MNIST-CoreML](https://github.com/ph1ps/MNIST-CoreML)

### Food101
Model: [Food101.mlmodel](https://github.com/ph1ps/Food101-CoreML/raw/master/Food101Prediction/Food101.mlmodel)

Description: Food classification

Author: [Philipp Gabriel](https://github.com/ph1ps)

Reference: [UPMC Food-101](http://visiir.lip6.fr/explore)

Example: [Food101-CoreML](https://github.com/ph1ps/Food101-CoreML)

### SentimentPolarity
Model: [SentimentPolarity](https://github.com/cocoa-ai/SentimentCoreMLDemo/raw/master/SentimentPolarity/Resources/SentimentPolarity.mlmodel)

Description: Sentiment Polarity Analysis

Author: [Vadym Markov](https://github.com/vadymmarkov)

Reference: [Epinions.com reviews dataset](http://boston.lti.cs.cmu.edu/classes/95-865-K/HW/HW3/)

Example: [SentimentCoreMLDemo](https://github.com/cocoa-ai/SentimentCoreMLDemo)

### VisualSentimentCNN
Model: [VisualSentimentCNN](https://drive.google.com/open?id=0B1ghKa_MYL6mZ0dITW5uZlgyNTg)

Description: Visual Sentiment Prediction

Author: [Image Processing Group - BarcelonaTECH - UPC](https://github.com/imatge-upc)

Reference: [From Pixels to Sentiment: Fine-tuning CNNs for Visual Sentiment Prediction](https://github.com/imatge-upc/sentiment-2017-imavis)

Example: [SentimentVisionDemo](https://github.com/cocoa-ai/SentimentVisionDemo)
