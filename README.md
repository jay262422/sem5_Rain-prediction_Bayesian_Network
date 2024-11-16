# Rain Prediction Using Bayesian Network

## Overview
This project implements a **Bayesian Network** to predict tomorrow’s rain probability based on historical weather data from Australia. The project demonstrates the use of **Probabilistic Graphical Models** (PGMs) to handle uncertainty and make predictions based on atmospheric variables such as temperature, humidity, and pressure.

## Features
- **Two Bayesian Network Models**: 
  - Manually constructed model (using parameter learning)
  - Automatically generated model (using structure learning and parameter learning)
- **Weather Dataset**: Utilizes 10 years of daily weather data from multiple Australian weather stations.
- **Prediction**: Forecasts the likelihood of rain tomorrow based on various atmospheric conditions.
- **Visualization**: A **Pygame GUI** for user interaction with the Bayesian Network.

## Dataset

The primary dataset used for this project is **weatherAUS.csv**, which contains historical weather data from Australia. It includes various features like temperature, humidity, pressure, and rain information.

### File Structure

- **`10_pro-2.jpeg`** and **`10_pro-5.jpeg`**: Images used in the report or project presentation.
- **`11_37-Article Text-2077-1-10-20220104 (1).pdf`**: Article used as reference for the project.
- **`11_Bayesian_network_model_for_monthly_rainfall_forecast (2).pdf`**: Paper discussing the Bayesian Network model applied to monthly rainfall forecasting.
- **`1_BasePapper.pdf`**: Base paper or reference document for Bayesian Networks.
- **`2_r_ads_g4_Abstract.pdf`**: Abstract or overview of the group’s approach.
- **`3_OLD_R_ADC_Group 4.mp4`** and **`4_ADS_G4.mp4`**: Video presentations or explanations of the project.
- **`5_DATASETweatherAUS.csv`**: Dataset used for training and testing the model.
- **`6_pgm_pro_final_for_our.csv`**: Processed dataset for model evaluation.
- **`7_ADS_g4_pgm_project.pdf`**: Full project report.
- **`8_9_pgm_pro_accuracy_comp.ipynb`**: Jupyter notebook for comparing model accuracy.
- **`8_9_pgm_pro_done_1.ipynb`**: Jupyter notebook detailing the implementation of the model.
- **`8_9_pgm_pro_game.ipynb`**: Jupyter notebook for implementing the Pygame.
- **`ADS_G4_PGM_Project_PPT.pdf`**: PowerPoint slides for the project presentation.
- **`README.md`**: This file.


## Models
- **Manually Constructed Network**: 
  - Built with predefined relationships and trained using **parameter learning** to calculate conditional probabilities.
  - Predicted tomorrow’s rain using **variable elimination**.
  
- **Automatically Generated Network**: 
  - Built using the **Hill Climbing K2 algorithm** for structure learning and **Bayesian Dirichlet equivalent uniform (BDeu)** for parameter learning.
  - Allows for automatic learning of the network structure and probabilistic relationships between variables.

## Accuracy
- **Manually Constructed Network**: 78.72% accuracy
- **Automatically Generated Network**: 79.16% accuracy

## Requirements
- Python 3.x
- Pygame (for the GUI)
- Libraries: `pgmpy`, `numpy`, `pandas`

## Setup
1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/bayesian-rain-prediction.git
    ```
2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```
3. Run the script to launch the Pygame GUI and interact with the Bayesian Network:
    ```bash
    python main.py
    ```

## Authors
- **Manav Yagnik** (AU2040040)
- **Vrutik Bavarva** (AU2040236)
- **Nand Patel** (AU2040183)
- **Jay Patel** (AU2040014)
