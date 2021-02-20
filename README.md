# Volcanic-Eruption-Prediction
This project achieves Volcanic Eruption Prediction by means of three different models CNN, DNN, LSTM and RF models to compare their results to get the least loss possible, which can be used for efficient prediction of the time left to next erruption of a certain volcano saving alot of lives and property. 

The approach we use for preprocessing of our data of 60001 of 10 different sensors readings for each volcano is Short Time Fourier Transform (STFT) function that is used to assess the sinusoidal frequency and phase content of the local signal parts as they shiftover time. We use this preprocessed data in three of our four models (CNN, DNN, LSTM).

However the forth model ,RF uses Auto-correlation to extract features depending on time-series waves for data preprocessing.

The four models achive good results in testing data that is further discussed in the paper.
