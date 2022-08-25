# ULMFiT-Sentiment
Applying a semi-supervised ULMFiT model to Twitter US Airlines Sentiment. 

<div align="center">
<img src="https://github.com/anmolpant/ULMFiT-Sentiment/blob/master/assets/airbus-a350-xwb-4k-passenger-plane-qantas-airlines-airbus-a350.jpg" >
</div>
<br>
Sentiment analysis is the interpretation and classification of emotions (positive, negative and neutral) within text data using text analysis techniques. Sentiment analysis tools allow businesses to identify customer sentiment toward products, brands or services in online feedback. It is one of the most basic techniques in Natural Language Processing to analyse the emotions and sentiments behind a specific piece of text.

In this project I was delegated the task of analysing the sentiments of the US-Airline-Twitter-Sentiment Dataset, but instead of using the conventional NLTK based approach and machine learning models, I was expected to use fastai's ULMFiT method that makes use of LSTMs and RNNs to perform the same. 

### Dataset Used

Twitter US Airline Sentiment: https://www.kaggle.com/crowdflower/twitter-airline-sentiment

### Method Deployed

Universal Language Model Fine-tuning for Text Classification (ULMFiT) method: https://www.aclweb.org/anthology/P18-1031.pdf

## Getting Started

The first few steps consisted of the usual data loading, splitting and pre-processing steps by plotting the various correlations between the different parameters given to us and filtering out the most important ones, followed by tokenization, removal of stop words and formulating regular expressions to weed out hashtags and links that might give the model an inaccurate picture of the dataset.

## Approach and Models

All the other details regarding the ULMFiT method for sentiment analysis can be found in the notebook itself, which is extremely well documented following the guidelines of the fellowship.ai team.

## Final Results and Scoring Metric Used

The scoring metric used here is 'accuracy'. Our model performs quite well having an overall accuracy of over 82% on the test set. It does a great job considering the fact that informal writings, like the ones on Twitter often do not make use of proper and conventional grammatical structures. Moreover, figures of speech such as 'sarcasm' are difficult to account for while feature engineering and are sometimes difficult to catch and recognize even for humans.

### Prerequisites

On my local machine, I've used: 
* Kaggle kernels - attributing to the sheer degree of convinience they provide when it comes to common Machine Learning Libraries and frameworks. , 
* python        : 3.7.6
* fastai        : 1.0.61
* fastprogress  : 0.2.3
* torch         : 1.5.1
* nvidia driver : 418.67
* torch cuda    : 10.1 
* torch cudnn   : 7603

### Hardware 
* nvidia gpus   : 1
* torch devices : 1
*  - gpu0      : 16280MB | Tesla P100-PCIE-16GB

## Contributing

Please feel free to fork the above repository and open an issue first before submitting a pull request. 

## Authors

* **Anmol Pant** - *Initial work* - (https://github.com/anmolpant)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

## Acknowledgments

* Shoutout to https://fellowship.ai/ for the opportunity to work on this problem.
