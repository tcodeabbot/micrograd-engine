🧠 Micrograd Engine

A lightweight automatic differentiation engine inspired by Andrej Karpathy’s micrograd
.
This project implements the fundamental building blocks behind deep learning frameworks like PyTorch — including tensors, backpropagation, and gradient computation — in just a few lines of Python.

🚀 Overview

The Micrograd Engine is a minimal autograd system built from scratch to demonstrate how neural networks compute and optimize using gradient-based learning.
It supports:

Scalar and tensor operations

Automatic differentiation via computational graphs

Backpropagation (reverse-mode autodiff)

Simple neural network layers and activation functions

Gradient-based optimization

This project aims to make backpropagation transparent and help others understand the math and mechanics behind modern deep learning frameworks.

🧩 Features

✅ Build dynamic computational graphs

✅ Track operations for automatic differentiation

✅ Perform gradient descent optimization

✅ Support basic arithmetic (+, -, *, /, **, tanh, exp, relu)

✅ Define and train small neural networks

🧠 How It Works

Each value in the computation is represented as a Value object containing:

A data scalar (.data)

A gradient (.grad)

A reference to the function that created it (._backward)

When you call .backward(), the engine performs reverse-mode autodiff, propagating gradients backward through the graph to compute partial derivatives automatically.
