# GRU Gate Interpretation: Understanding Selective Memory
# Overview

This project investigates how Gated Recurrent Units (GRUs) manage memory in sequential data. Instead of focusing solely on model performance, the work examines the internal behaviour of the update gate and reset gate to understand how the model selectively retains relevant information.

A synthetic sequence classification task is used to provide full control over the signal and noise in the data. This enables a direct comparison between:

a clean setting with a clear informative signal
a noisy setting with large distractor inputs

The results demonstrate how GRU gating mechanisms adapt to increasing task complexity.

# Project Structure
24133600_code.ipynb – Main notebook containing data generation, model training, and visualisation
figures/ – Generated plots used in the tutorial
requirements.txt – List of required Python packages
README.md – Project documentation
Requirements

# The project requires Python 3 and the following libraries:

numpy
matplotlib
torch

# Install dependencies using:

pip install -r requirements.txt
How to Run
Clone or download the repository.
Ensure all dependencies are installed.
Open the Jupyter notebook:
jupyter notebook 24133600_code.ipynb
Run all cells in order.
What the Code Does

# The notebook performs the following steps:

Dataset Generation
Creates synthetic sequences where only one timestep determines the label.
Model Implementation
Defines a custom GRU model that exposes update and reset gate values.
Training
Trains separate models on clean and noisy datasets.
Visualisation

# Generates:

sample input sequences
training curves
gate activation heatmaps
aggregate gate comparison plots
