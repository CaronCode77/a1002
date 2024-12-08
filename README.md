<p align="center" style="font-size:50px; font-weight:bold;">
<strong>AIDI Machine Learning Programming - Research Project</strong>
</p>

<p align="center" style="font-size:24px; font-weight:bold;">
<strong>[Predicting Stock Market Time-Series Data]</strong>
</p>
<p align="center" style="font-size:20px;">
<strong>CNN-LSTM Neural Network Model</strong><br>
vs <br>
<strong>Stacked-LSTM NN Model</strong><br>
vs <br>
<strong>BiDirectional-LSTM NN Model</strong>
</p>

## Overview
This school project researches stock market time series data price prediction, with a focus on an article which uses a hybrid deep learning model combining Convolutional Neural Networks (CNN) and Long Short-Term Memory (LSTM) to predict stock market prices in comparison to other machine learning models like Random Forest, LBL-LSTM, k-NN Regression, SVM, and more. The article highlights the challenges of highly volatile and complex nature of stock market pricing and proposes that their CNN-LSTM machine learning models produce superior predictions on a comparison of accuracy markers.  

Our task in this project is to replicate the referenced code in article and create an upgraded version of LSTM machine learning model that will increase the model's performance.  Given the vast amount of options available to us and reduced time to test and train deep learning models we have narrowed down our possible enhancements to a Stacked-LSTM model and a Bidirectional-LSTM model.  

## Research Paper on Time Series Forecasting:
https://arxiv.org/pdf/2305.14378   
Published: May 21st, 2023

## Relevant DataSet: 
https://github.com/Circle-1/Stock-X/blob/main/data/NIFTY/ITC.csv   
Source: NIFTY (National Stock Exchange Fifty, an index representing the top 50 companies listed on the National Stock Exchange (NSE) of India)

## CNN-LSTM Model
Convolutional Neural Network with Long Short-Term Memory combines a CNN for feature extraction and a LSTM network for sequential data modeling. The CNN layers extract spatial features, flattened or reshaped features are then passed to LSTM layers to model time-dependent patterns.    

The replicated research paper python script was selected and deployed against the relevant dataset.  Assessing the model accuracy and precision we used the standard Mean Absolute Error and Mean Squared Error calculations which were as follows:   

Mean Absolute Error: 7.920070029978962   
Mean Squared Error: 147.60807218374518   

## Stacked-LSTM Models
In "stacked" LSTM models multiple LSTM layers are stacked on top of each other allowing the model to learn more complex features hierarchically.  With multiple layers it can learn both simple and complex temporal dependencies in sequential data like stock prices. Stacked models are capable of handling multivariant data features such as OHLC and indicators like RSI.  Lastly, deeper layers can capture interactions in data such as price reversals and trends.  

A stacked-LSTM model was created from the research paper python script and deployed against the relevant dataset.  Assessing the model accuracy and precision we used the standard MAE and MSE calculations which were as follows:   

Mean Absolute Error: 4.685022011912624   
Mean Squared Error: 44.915101133343875 

## Bidirectional-LSTM Models
Unlike standard LSTM, Bidirectional LSTM processes sequences in forward and backward directions better capturing swings in time-series data.  Capturing these sequences allows for better predictions on for example, RSI indicating an upcoming trend reversal.  Ultimately though, bidirectional is very useful when the data has cyclical or seasonal patterns that need backward context for better predictions.  

A bidirectional-LSTM model was created from the research paper python script and deployed against the relevant dataset.  Assessing the model accuracy and precision we used the standard MAE and MSE calculations which were as follows:   

Mean Absolute Error: 3.953184636197867   
Mean Squared Error: 30.931766687269413    

## Conclusion   
This project set out to enhance machine learning model for Predicting Stock Market Time-Series Data building upon the CNN-LSTM hybrid deep learning architecture presented in the referenced research paper. Through  replication and analysis and development and evaluation of LSTM variants  significant improvements in prediction accuracy have been achieved.   

The CNN-LSTM model demonstrated the utility of combining feature extraction with sequence modeling. However its performance metrics with a MAE of 7.92 and a MSE of 147.61 left room for improvement.   

Extending this baseline, the Stacked-LSTM model introduced hierarchical learning capturing both simple and complex temporal dependencies and resulted in a significant reduction of error rates with an MAE of 4.69 and an MSE of 44.92.  This highlights the models ability to handle multivariate features and uncover intricate patterns in stock price movements.   

The Bidirectional-LSTM model further enhanced prediction accuracy by incorporating both forward and backward sequence processing. This approach enabled the model to better capture patterns, particularly detecting price reversals and trend changes. With an MAE of 3.95 and an MSE of 30.93 the Bidirectional-LSTM emerged as the most accurate model tested in this project.   \






