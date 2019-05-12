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
<img src="https://github.com/mrizwan18/Cats-Vs-Dogs-Prediction-using-CNN-on-altered-dataset/blob/master/Summary.JPG" />
</p>
<h1>4. Results:</h1>
<p>Maximum accuracy computed over the period of 30 epochs is 94%. The model was trained for 50 epochs and the weights with least loss were used for making the final predictions. The price movement is a 0-1 classification problem and hence categorical cross entropy, which reduces to binary cross entropy in this case is used a measure of loss. The results of minimizing the loss over the course of 50 epochs are as shown in Figure 5. Initially the training loss is very high and test loss is moderate. After around 8 epoch test loss achieves a minimum value and the model is well fitted at this stage. </p>
 
<p><b>Test accuracy fluctuates over time but peaks at around 30th epoch is of 94% and validation accuracy is roughly <i>86%<i></b>
 </p>

<h1>5. Conclusion:</h1>
<p>Since our objective was to increase the accuracy on the dataset provided by optimally tuning the parameters, it is obvious that the model behaved well even for an altered version of dataset</p>


<h1>6. References:</h1>
<p>1.	<a href="https://github.com/yumoxu/stocknet-dataset"> <b>Data Set </b></a>
2.	<a href="http://cs229.stanford.edu/proj2011/GoelMittal-StockMarketPredictionUsingTwitterSentimentAnalysis.pdf"> <b>Twitter Sentiment Analysis</b></a>
3.	<a href="https://medium.com/@alexrachnog/neural-networks-for-algorithmic-trading-2-1-multivariate-time-series-ab016ce70f57"> <b>Multivariate Time Series</b> </a></p>


