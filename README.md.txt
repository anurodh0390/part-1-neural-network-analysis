Part 1: Neural Network Analysis for Churn Prediction
Project Overview
The goal of this project is to build a neural network model that can predict whether a customer will leave a company (churn). The process involved data cleaning, training the model, and testing different configurations to see which settings provide the highest accuracy.

Model Performance and Experiments
I conducted 4 different experiments to find the best configuration for the model:

Base Model (16 Neurons, ReLU, 0.001 Learning Rate): 97.75% Accuracy

Deeper Model (32 and 16 Neurons): 98.75% Accuracy (Best Result)

High Learning Rate (0.1): 98.00% Accuracy

Tanh Activation Function: 98.25% Accuracy

The highest accuracy was achieved by the Deeper Model (32 and 16 neurons), showing that adding more hidden layers helped the model learn the data more effectively.

Final Reflection
Weights and Biases: Weights determine the importance of each feature (like monthly charges). Biases give the model flexibility to adjust its decisions to better fit the data.

Activation Function: I used ReLU and Tanh functions. These allow the model to understand complex patterns that cannot be captured by simple linear formulas.

Learning Rate: During the experiment, I found that a high learning rate (0.1) makes training faster but can be unstable. The rate of 0.001 provided the most stable and reliable training.

Overfitting and Underfitting: The training and testing accuracies are very close (~98%). This indicates that the model has generalized well and is not simply memorizing the training data (no overfitting).

Repository Structure
notebook.ipynb: Contains all the Python code and analysis.

requirements.txt: Lists the libraries needed to run the project.

results/: This folder contains the comparison tables and performance graphs.