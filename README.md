# Volcanic-Eruption-Prediction
This repository is an answer to Volcanic Eruption Prediction Competition: https://www.kaggle.com/c/predict-volcanic-eruptions-ingv-oe

Original data: https://www.kaggle.com/c/predict-volcanic-eruptions-ingv-oe/data

This project achieves Volcanic Eruption Prediction by means of three different models CNN, DNN, LSTM and RF models to compare their results to get the least loss possible, which can be used for efficient prediction of the time left to next erruption of a certain volcano saving alot of lives and property. 

The approach we use for preprocessing of our data of 60001 of 10 different sensors readings for each volcano is Short Time Fourier Transform (STFT) function that is used to assess the sinusoidal frequency and phase content of the local signal parts as they shiftover time. We use this preprocessed data in three of our four models (CNN, DNN, LSTM). The three of them are uploaded as jupitar notebooks. The preprocessing code can be found within the CNN model notebook.

As for the forth model RF: 
There are two codes, “Pre-Processing” for pre-processing data with auto-correlation to extract features 

   “RF-ModelTraining” for training random forest model on preprocessed data. 

Note: pre-processing data takes long time around 4.5 hours. 

Pre-processed data are here named for training and testing sensors  readable with pickle library: www.kaggle.com/dataset/28b1198b187c9ff000c6487d0ba556f014063552387b0687795e022cca69f544

labels.txt file: contains time to eruption data. 
test_labels.txt file : contains segment_id (names of volcanos that we are predicting its time to eruption)
 
Codes are uploaded as txt files.  please run it on Kaggle notebook.

The four models achive good results in testing data that is further discussed in the paper.
