# Time Series Anomaly Detection
Anomaly Detection — is the identification of rare items, events, or patterns that significantly differ from the majority of the data.
![anomaly graph](https://miro.medium.com/max/800/0*bmXOsrnZgb4FAdMU)
## Dataset
 **The Numenta Anomaly Benchmark (NAB)**: 
- Contains many files with different metrics from different places. It is in the nature of metrics — being ordered in time.
- From NAB we decided to use Real CPU utilization from AWS Cloudwatch metrics for Amazon Relational Database Service. These metrics are saved in csv format and the exact timestamps of anomalies in them (let’s call it labels) are saved in json format.
## Model
- <b>ARIMA statistical model as a baseline </b> — this is the classic auto-regression model that is made exactly for the time series.
- <b>Convolutional Neural Network </b> — such neural networks are usually used for image processing, but if you dig deeper into them, you may find that they actually look for the patterns in the images. Our time series also consists of patterns
- <b>Long Short-Term Memory Neural Network </b> — this type was designed especially for time-related data
## Tools
- <b> Google Colab </b> as working environment for .ipynb files.
- <b> Scikit-Learn </b> for some data preprocessing.
- <b> Statsmodel </b> library for ARIMA model.
- <b> PyTorch </b> for neural networks.
- <b> Plotly </b> for plots and graphs.
