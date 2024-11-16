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

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
