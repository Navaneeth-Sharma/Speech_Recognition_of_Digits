# Speech Recognition of Digits
## Aprroach
This project of recognizing digit and converting it to text uses Signal processing techniques such as MFCC and other Advanced Signal Processing techniques for the preprocessing of the data. Then the Preprocessed data is used by the Neural Network algorithms to learn the pattern or structure of the sound.This Project can broadly divide into 4 main steps. Those
steps are –
1. Collecting the Voice Data of Digits
2. Preprocessing the Data using Advanced Signal Processing techniques
3. Training by preprocessed data and creating a model
4. Validating and Testing the Model
<br>
&nbsp;&nbsp;&nbsp;&nbsp;The data for this project is collected from kaggle.com, which is a popular websites for
Projects related to the Machine Learning and Data Science. The dataset has about 3000
samples i.e about 50 dataset for each digit.The Clean version of Data is <a href='https://drive.google.com/file/d/1fNwxwDvunG9VI8cbM6Dkjfl0fiOUM5nr/view?usp=sharing'>here</a>. The 2nd step i.e preprocessing data is done
through ASP techniques such as Mel Frequency Cepstral Coefficients (MFCCs). These
techniques are generally used in signal processing for studding the feature of the signal. Our
Approach is to convert the Speech signal to MFCC images and then to feed that to train the
Model. The Convolutional Neural Networks (CNN) algorithm is used to train the model.
CNN uses a basic Image processing technique of convolution of 2 images. Here Conv 2D is
used, which is powerful for the images. After Creation of the model, recorded voice input is
fed to the model, and the model predicts digit of the given Voice signal. This project uses
python for developing the model, due to the vastness of Deep learning libraries present for
python.

## Implementation
The SRD.ipynb contains the preprcessing of the data. Here Mel Frequency Cepstrum Coefficients(MFCC) is used to convert the speech data points to MFCC images. This implies the problem statement is converted from Speech Recognition to Image Recognition. Then it is Divided into training and validation data for analysing the metrics. Then the Data is fed to the Model which looks like 

![alt text](https://github.com/Navaneeth-Sharma/Speech_Recognition_of_Digits/blob/main/model_summary.jpg)

The Adam Optimizer is used for Optimization on the Weights, Categorical Loss (since Categorical Data) and batch size is about 64.

## Results and Analysis
When audio signal is played our neural network model identifies the number and displays it
on the screen. Our model works with 98% percent accuracy. The Execution time is about
200ms which makes the model light weight and also fast enough for the real time
deployment.
<br>
&nbsp;&nbsp;&nbsp;&nbsp;Thus it is analyzed that MFCC is very powerful for the word detection as it produces unique
images for unique sounds irrespective of the pitch. Converting Speech to MFCC image has
raised accuracy by 20% which is critical for the deployment. Use of CNN has prevented the
model from getting over fitted and as drastically reduced number of computations unlike in
other neural networks. Thus it is verified that CNN is reliable and effective when we use
image training data. Vast libraries of python like keras, librosa etc used has simplified the
design of the model. Hyper tuning parameters like batch size, learning rate and other
parameters have been observed and noted down.
<br>
Model is trained with 2700 samples with an accuracy of 98.6%
and validated with 300 samples with an accuracy of 92%

