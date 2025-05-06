# HTTP-Payload-Anomaly-Detection-LSTM-Without-Attention-
This project implements an LSTM-based model to detect anomalies in HTTP payloads. The objective is to identify abnormal network behavior that may indicate security threats, such as intrusions or attacks, without using attention mechanisms.
 Overview
Model: LSTM Encoder-Decoder

Input: HTTP Payloads (sequences)

Goal: Anomaly detection by reconstructing normal payloads and identifying deviations

Comparison: This implementation serves as a baseline for further enhancement using attention and Transformer-based models.


Without_Attention_(LSTM).ipynb: Jupyter Notebook with model training, evaluation, and visualization.

Train_data.csv & Test_data.csv: Input datasets used for training and testing the model.
Installation
Clone the repository:
git clone https://github.com/yourusername/http-payload-anomaly-lstm.git
cd http-payload-anomaly-lstm
Install dependencies:
pip install -r requirements.txt
Model Architecture
Encoder: LSTM layers encoding the payload

Decoder: LSTM layers attempting to reconstruct the original input

Loss Function: Mean Squared Error (MSE)

Anomaly Detection: Based on reconstruction error threshold

 Results
The model distinguishes between normal and anomalous payloads with a threshold on reconstruction loss.

Plots and metrics (e.g., ROC, confusion matrix) are included in the notebook.
