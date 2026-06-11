# Nvidia 6G link budget simulator with ML prediction

- a wireless link quality simulator built with the nvidia 6g sionna ai model
- includes a machine learning model that predicts the throughput of a network from signal connections

# Project overview

The project simulates a wireless communication link across different signal to noise ratio conditions and trains a random forest model to predict the throughput of the link

# Info

- Model: Random forest (100 trees)
- 400 training samples
- 100 test samples
- RMSE of 2.28 mbps
- Top predictive feature: SNR in db

# What I built

- Simulated SNR vs BER and SNR vs throughput curves using shannon capacity and BPSK modulation models
- Added realistic noise to simulate variabliltity that comes in real world scenarios
- Trained a random forest regressor to predict throughput from SNR and BER
- Got 2.28 mbps RMSE between a 0-200 range
- Identified SNR as the dominant factor 

# How to run

- Clone this repo
- Create and activate a virtual environment
- Install the sionna, jupyter, etc dependencies
- Open the notebook in notebooks/link_budget_simulator.ipynb and open it in Jupyterlab
- Run all cells top to bottom for results

