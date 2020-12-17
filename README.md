# Speech_Recognition_of_Digits
This project of recognizing digit and converting it to text uses Signal processing techniques such as MFCC and other Advanced Signal Processing techniques for the preprocessing of the data. Then the Preprocessed data is used by the Neural Network algorithms to learn the pattern or structure of the sound.This Project can broadly divide into 4 main steps. Those
steps are –
1. Collecting the Voice Data of Digits
2. Preprocessing the Data using ASP techniques
3. Training by preprocessed data and creating a model
4. Testing the Model
The data for this project is collected from kaggle.com, which is a popular websites for
Projects related to the Machine Learning and Data Science. The dataset has about 3000
samples i.e about 50 dataset for each digit. The 2nd step i.e preprocessing data is done
through ASP techniques such as Mel Frequency Cepstral Coefficients (MFCCs). These
techniques are generally used in signal processing for studding the feature of the signal. Our
Approach is to convert the Speech signal to MFCC images and then to feed that to train the
Model. The Convolutional Neural Networks (CNN) algorithm is used to train the model.
CNN uses a basic Image processing technique of convolution of 2 images. Here Conv 2D is
used, which is powerful for the images. After Creation of the model, recorded voice input is
fed to the model, and the model predicts digit of the given Voice signal. This project uses
Speech Recognition of Digits
Department of Electronics & Communication Engineering Page 2
python for developing the model, due to the vastness of Deep learning libraries present for
python.