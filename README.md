# ML_03 — Logistic Regression From Scratch

## Overview
This project builds a classifier from scratch that identifies whether 
a tumor is benign or malignant.

## Objective
Using logistic regression, I created a classification model. It is 
similar to linear regression, but here we need a yes/no answer (0 or 1), 
so we use the sigmoid function for that. We use log loss to find the 
cost, so the model works harder on bigger mistakes.

## Concept
The predict function gives an answer, and sigmoid converts that answer 
into the range 0 to 1 (a probability). Then we find the cost means how far 
the prediction is from the true answer — and compute the gradient to 
reduce the cost.

(Note: logistic regression is a CLASSIFICATION algorithm, despite the 
word "regression" in its name , the sigmoid is what makes it classify.)

## Dataset
Breast Cancer dataset from sklearn. It has 569 patients, 30 features, 
and a label = benign (0) / malignant (1).

## Steps Performed
- Load data
- Separate features and target
- Build sigmoid function
- Predict the answer and pass it through sigmoid
- Find cost (log loss)
- Compute gradient in a training loop

## Key Concepts
- **Log loss** — used so big mistakes get penalized properly
- **Feature scaling** — so features with a small scale are not 
  neglected by the model

## Results
The model reached 95.6% accuracy.
(Note: this was tested on the training data, so it is not a fully 
honest measure — testing on unseen data would confirm true performance.)

## Tech Stack
- Python
- NumPy
- sklearn (for the dataset and feature scaling)

## What I Learned
My understanding of ML improved a lot — especially how a classifier 
learns using sigmoid, log loss, and gradient descent. This will help 
me build my future projects.
