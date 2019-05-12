# Cats Vs Dogs Prediction using CNN on altered dataset
In this project a CNN is trained to predict the label of image as cat or dog from an altered dataset. This project is actually an example of parameter tuning to produce >80% accuracy.
<h1>1. Introduction:</h1>
<p>Cats vs Dogs prediction is a very well known problem in Convolutional Neural Network learning and has been solved efficiently by a lot of people. This project focuses more on the dataset alteration problem where the conservative methods won't produce good accuracy. So the project is a fine example of paramtere tuning to acheive a better accuracy</p>

<h1>2. Dataset:</h1>
<p>The dataset used in this project is an altered version of original Kaggle dataset and a link is provided to the altered version at the end. It includes 25000 total images of cats and dogs. Training data includes 8000 images of cats and dogs respectively in seperate folders. Then the validation data is of 3500 images of each animal. </p>
<h1>Preprocessing:</h1>
<p>Preprocessing includes the data augmentation, that <b>rescales, applies shear range, zoom range and horizontal flip.</b></p>
<h1>3. Methodology: </h1>
<p>CNN is used with following summary:</p>
</br>
<p>
<img src="" />
</p>
 
<h1>Model:</h1>
<p>For the purpose of prediction we have used CNN model. Convolutional neural networks are deep artificial neural networks that are used primarily to classify images (e.g. name what they see), cluster them by similarity (photo search), and perform object recognition within scenes. They are algorithms that can identify faces, individuals, street signs, tumors, platypuses and many other aspects of visual data. CNN has been successful in various text classification tasks. In KimY’s report, Convolutional Neural Networks for Sentence Classification, the author showed that a simple CNN with little hyperparameter tuning and static vectors achieves excellent results on multiple benchmarks – improving upon the state of the art on 4 out of 7 tasks. A 1D CNN is very effective when you expect to derive interesting features from shorter (fixed-length) segments of the overall data set and where the location of the feature within the segment is not of high relevance. This applies well to the analysis of time sequences of sensor data (such as gyroscope or accelerometer data). It also applies to the analysis of any kind of signal data over a fixed-length period (such as audio signals). Another application is NLP (although here LSTM networks are more promising since the proximity of words might not always be a good indicator for a trainable pattern). Mainly we choose CNN because of flexibility and interpretability of hyperparameters (convolutional kernel etc.) and performance similar to RNNs, better than MLP with much faster training. The architecture used has two 1d convolution layers with activation set to Leaky Relu and dropout set to 0.5. It is followed y a fuly connected layer with 64 neurons and activation set to Leaky Relu. Last layer is a Softmax layer. We have used Nadam as the optimizer with learning rate set to 0.002. Batch size of 128 is used for 50 epochs. </p>
 
<h1>4. Results:</h1>
<p>Maximum accuracy computed over the period of 50 epochs is 70%. The model was trained for 50 epochs and the weights with least loss were used for making the final predictions. The price movement is a 0-1 classification problem and hence categorical cross entropy, which reduces to binary cross entropy in this case is used a measure of loss. The results of minimizing the loss over the course of 50 epochs are as shown in Figure 5. Initially the training loss is very high and test loss is moderate. After around 8 epoch test loss achieves a minimum value and the model is well fitted at this stage. </p>
 
<b>Test accuracy fluctuates over time but peaks at around 8th epoch and maximum accuracy of 0.699999988079071 or roughly <i>70%<i> is achieved at that stage.</b>

<h1>5. Conclusions And Future Work:</h1>
<p>Multivariate Time Series Deep Learning holds great potential for stock price predictions and has been shown to achieve better results than techniques relying solely on price data by supplementing it with Twitter Sentiment data. An accuracy of 70% for predicting price change direction has been obtained beating comparable models that relies on just price data. Our results are in conjucture with past experimental works that Twitter data can be used to predict movement of stock prices.
Finally, its worth mentioning that our analysis doesn’t take into account many factors. Firstly, our dataset doesn’t really map the real public sentiment, it only considers the twitter using, English speaking people. It’s possible to obtain a higher correlation if the actual mood is studied. It maybe hypothesized that people’s mood indeed affect their investment decisions, hence the correlation. But in that case, there’s no direct correlation between the people who invest in stocks and who use twitter more frequently, though there certainly is an indirect correlation - investment decisions of people may be affected by the moods of people around them, ie. the general public sentiment. All these remain as areas of future research. 
It is worth noting that the model uses Twitter information for stock market as a whole instead of targeted recognized sources to make trading decisions for individual stocks which restricts its performance and at the same time makes the implementation simplistic. Also, sentiment can be divided into more categories of mood to better predict correlation between public sentiment and stock price. News data can also incorporated with tweet data making prediction more accurate. Also, the high frequency price data and live news feed can be used to make a real time High Frequency Trading (HFT) system using the architecture of proposed model.
The test accuracy can be improved by using more sophisticated models such as LSTM in the future. 
To sum it up, this work provides an exposure into the application of Multimodal and Multitask learning to financial time series data. The positive results obtained validate the credibility of model for more complex tasks.</p>


<h1>6. References:</h1>
<p>1.	<a href="https://github.com/yumoxu/stocknet-dataset"> <b>Data Set </b></a>
2.	<a href="http://cs229.stanford.edu/proj2011/GoelMittal-StockMarketPredictionUsingTwitterSentimentAnalysis.pdf"> <b>Twitter Sentiment Analysis</b></a>
3.	<a href="https://medium.com/@alexrachnog/neural-networks-for-algorithmic-trading-2-1-multivariate-time-series-ab016ce70f57"> <b>Multivariate Time Series</b> </a></p>


