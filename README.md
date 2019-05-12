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
<p><b>Test accuracy fluctuates over time but peaks at around 30th epoch as 94% and validation accuracy is roughly <i>86%<i></b>
<img src="https://github.com/mrizwan18/Cats-Vs-Dogs-Prediction-using-CNN-on-altered-dataset/blob/master/acc.JPG" />
 </p>

<h1>5. Conclusion:</h1>
<p>Since our objective was to increase the accuracy on the dataset provided by optimally tuning the parameters, it is obvious that the model behaved well even for an altered version of dataset</p>


<h1>6. References:</h1>
<p>1.	<a href="https://www.kaggle.com/kernels"> <b>Kaggle Kernel for computation </b></a>
2.	<a href="https://medium.com/data-science-101/creating-a-simple-dog-cat-image-classifier-using-keras-7dffdeea0f66"> <b>Medium.com Article</b></a>
3.	<a href="https://drive.google.com/file/d/1fk-rBgurmtJGkgpmdk0QbVB2iZe8fWl9/view"> <b>Altered Dataset</b> </a></p>


