<img src="core-ml.png" align="left" width="64"> 

# Awesome Core ML models [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

This repository has a collection of Open Source machine learning models which work with Apples **Core ML** standard.

Apple has published some of their own models. They can be downloaded [here](https://developer.apple.com/machine-learning/).
Those published models are: **SqueezeNet, Places205-GoogLeNet, ResNet50, Inception v3, VGG16** and will not be republished in this repository.

## Contributing
If you want your model added simply create a pull request with your repository and model added. In order to keep the quality of this repository you have to conform to this project structure (taken from **@hollance**).

```
├── Convert
    ├── coreml.py
    ├── mobilenet_deploy.prototxt
    └── synset_words.txt
```

There has to be a **Convert** directory with a Python script and additional data to reproduce this model on your own. If your model requires a huge amount of space please include a script which downloads those files.

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

This is a template for the README to copy:
```
### Name of your model
**Model:** [Model.mlmodel](link for downloading) <br />
**Description:** Short description <br />
**Author:** [Author](https://github.com/author) <br />
**Reference:** [Name of reference](URL to reference) <br />
**Example:** [Your example project](URL to example project) <br />
```
## Models

### MobileNet
**Model:** [MobileNet.mlmodel](https://github.com/hollance/MobileNet-CoreML/raw/master/MobileNet.mlmodel) <br />
**Description:** Object detection, finegrain classification, face attributes and large scale geo-localization <br />
**Author:** [Matthijs Hollemans](https://github.com/hollance) <br />
**Reference:** [MobileNets: Efficient Convolutional Neural Networks for Mobile Vision Applications](https://arxiv.org/abs/1704.04861v1) <br />
**Example:** [MobileNet-CoreML](https://github.com/hollance/MobileNet-CoreML) <br />

### MNIST
**Model:** [MNIST.mlmodel](https://github.com/ph1ps/MNIST-CoreML/raw/master/MNISTPrediction/MNIST.mlmodel) <br />
**Description:** Handwritten digit classification <br />
**Author:** [Philipp Gabriel](https://github.com/ph1ps) <br />
**Reference:** [MNIST handwritten digit database](http://yann.lecun.com/exdb/mnist/) <br />
**Example:** [MNIST-CoreML](https://github.com/ph1ps/MNIST-CoreML) <br />

### Food101
**Model:** [Food101.mlmodel](https://drive.google.com/open?id=0B5TjkH3njRqnVjBPZGRZbkNITjA) <br />
**Description:** Food classification <br />
**Author:** [Philipp Gabriel](https://github.com/ph1ps) <br />
**Reference:** [UPMC Food-101](http://visiir.lip6.fr/explore) <br />
**Example:** [Food101-CoreML](https://github.com/ph1ps/Food101-CoreML) <br />

### SentimentPolarity
**Model:** [SentimentPolarity](https://github.com/cocoa-ai/SentimentCoreMLDemo/raw/master/SentimentPolarity/Resources/SentimentPolarity.mlmodel) <br />
**Description:** Sentiment Polarity Analysis <br />
**Author:** [Vadym Markov](https://github.com/vadymmarkov) <br />
**Reference:** [Epinions.com reviews dataset](http://boston.lti.cs.cmu.edu/classes/95-865-K/HW/HW3/) <br />
**Example:** [SentimentCoreMLDemo](https://github.com/cocoa-ai/SentimentCoreMLDemo) <br />

### VisualSentimentCNN
**Model:** [VisualSentimentCNN](https://drive.google.com/open?id=0B1ghKa_MYL6mZ0dITW5uZlgyNTg) <br />
**Description:** Visual Sentiment Prediction <br />
**Author:** [Image Processing Group - BarcelonaTECH - UPC](https://github.com/imatge-upc) <br />
**Reference:** [From Pixels to Sentiment: Fine-tuning CNNs for Visual Sentiment Prediction](https://github.com/imatge-upc/sentiment-2017-imavis) <br />
**Example:** [SentimentVisionDemo](https://github.com/cocoa-ai/SentimentVisionDemo) <br />

### AgeNet
**Model:** [AgeNet](https://drive.google.com/file/d/0B1ghKa_MYL6mT1J3T1BEeWx4TWc/view?usp=sharing) <br />
**Description:** Age Classification <br />
**Author:** [Gil Levi and Tal Hassner](http://www.openu.ac.il/home/hassner/projects/cnn_agegender/) <br />
**Reference:** [Age and Gender Classification using Convolutional Neural Networks](http://www.openu.ac.il/home/hassner/projects/cnn_agegender/CNN_AgeGenderEstimation.pdf) <br />
**Example:** [FacesVisionDemo](https://github.com/cocoa-ai/FacesVisionDemo) <br />

### GenderNet
**Model:** [GenderNet](https://drive.google.com/file/d/0B1ghKa_MYL6mYkNsZHlyc2ZuaFk/view?usp=sharing) <br />
**Description:** Gender Classification <br />
**Author:** [Gil Levi and Tal Hassner](http://www.openu.ac.il/home/hassner/projects/cnn_agegender/) <br />
**Reference:** [Age and Gender Classification using Convolutional Neural Networks](http://www.openu.ac.il/home/hassner/projects/cnn_agegender/CNN_AgeGenderEstimation.pdf) <br />
**Example:** [FacesVisionDemo](https://github.com/cocoa-ai/FacesVisionDemo) <br />

### CNNEmotions
**Model:** [CNNEmotions](https://drive.google.com/file/d/0B1ghKa_MYL6mTlYtRGdXNFlpWDQ/view?usp=sharing) <br />
**Description:** Emotion Recognition <br />
**Author:** [Gil Levi and Tal Hassner](http://www.openu.ac.il/home/hassner/projects/cnn_emotions/) <br />
**Reference:** [Emotion Recognition in the Wild via Convolutional Neural Networks and Mapped Binary Patterns](http://www.openu.ac.il/home/hassner/projects/cnn_emotions/LeviHassnerICMI15.pdf) <br />
**Example:** [FacesVisionDemo](https://github.com/cocoa-ai/FacesVisionDemo) <br />

### NamesDT
**Model:** [NamesDT](https://github.com/cocoa-ai/NamesCoreMLDemo/raw/master/Names/Resources/NamesDT.mlmodel) <br />
**Description:** Gender Classification from first names <br />
**Author:** [http://nlpforhackers.io](http://nlpforhackers.io) <br />
**Reference:** [Is it a boy or a girl? An introduction to Machine Learning](http://nlpforhackers.io/introduction-machine-learning/) <br />
**Example:** [NamesCoreMLDemo](https://github.com/cocoa-ai/NamesCoreMLDemo) <br />

### Oxford102
**Model:** [Oxford102](https://drive.google.com/file/d/0B1ghKa_MYL6meDBHT2NaZGxkNzQ/view?usp=sharing) <br />
**Description:** Flower Classification <br />
**Author:** [Jimmie Goode](https://github.com/jimgoo) <br />
**Reference:** [Classifying images in the Oxford 102 flower dataset with CNNs](http://jimgoo.com/flower-power/) <br />
**Example:** [FlowersVisionDemo](https://github.com/cocoa-ai/FlowersVisionDemo) <br />

### FlickrStyle
**Model:** [FlickrStyle](https://drive.google.com/file/d/0B1ghKa_MYL6maFFWR3drLUFNQ1E/view?usp=sharing) <br />
**Description:** Image Style Classification <br />
**Author:** [Sergey Karayev](https://gist.github.com/sergeyk) <br />
**Reference:** [Recognizing Image Style](http://sergeykarayev.com/files/1311.3715v3.pdf) <br />
**Example:** [StylesVisionDemo](https://github.com/cocoa-ai/StylesVisionDemo) <br />
