<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MNIST Digit Classifier</title>
</head>
<body>
    <h1>MNIST Digit Classifier</h1>
    <p>This project implements a classifier for handwritten digits from the MNIST dataset. The classifier uses a neural network to recognize digits from 0 to 9 with high accuracy.</p>
 <h2 id="introduction">Introduction</h2>
    <p>The MNIST database is a large database of handwritten digits commonly used for training various image processing systems. It has a training set of 60,000 examples and a test set of 10,000 examples. This project aims to build a classifier to accurately identify these handwritten digits.</p>

   <h2 id="installation">Installation</h2>
    <p>To install the necessary packages, run:</p>
    <pre>
    pip install -r requirements.txt
    </pre>

    <h2 id="usage">Usage</h2>
    <p>To train the model, run:</p>
    <pre>
    python scripts/train.py
    </pre>
    <p>To evaluate the model, run:</p>
    <pre>
    python scripts/evaluate.py
    </pre>

    <h2 id="model-architecture">Model Architecture</h2>
    <p>The model is a simple neural network with the following layers:</p>
    <ul>
        <li>Input layer: Flattening the 28x28 image into a 784-dimensional vector</li>
        <li>Hidden layer 1: Dense layer with 128 units and ReLU activation</li>
        <li>Hidden layer 2: Dense layer with 64 units and ReLU activation</li>
        <li>Output layer: Dense layer with 10 units (one for each digit) and softmax activation</li>
    </ul>

    <h2 id="training">Training</h2>
    <p>The model is trained using the Adam optimizer and categorical cross-entropy loss. Training is performed over 10 epochs with a batch size of 32.</p>

    <h2 id="evaluation">Evaluation</h2>
    <p>The model is evaluated on the test set using accuracy as the metric. The evaluation script prints the accuracy of the model on the test set.</p>

    <h2 id="results">Results</h2>
    <p>The model achieves a high accuracy on the test set.</p>
