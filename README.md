  # Linear Regression from Scratch in C++

A lightweight, dependency-free implementation of single-variable linear regression using **Gradient Descent**. This project predicts real estate property prices based on square footage, built entirely from scratch in C++ to demonstrate the core mathematics behind machine learning optimization.

## 🚀 Features
* **Zero External ML Libraries:** Implements the core gradient descent loop, partial derivatives, and cost calculations using only standard C++.
* **Feature & Target Scaling:** Normalizes both $X$ (square footage) and $Y$ (prices) to prevent floating-point overflow and ensure algorithm convergence.
* **Early Stopping:** Automatically halts the training loop when the weight and bias updates become negligibly small, optimizing computational efficiency.
* **Memory Efficient:** Uses constant references for large datasets to prevent unnecessary memory reallocation during training.

## 🧠 The Mathematics
The algorithm fits a line of best fit using the linear equation:
$$y = wx + b$$

Where:
* y is the predicted price.
* x is the square footage.
* w is the weight (slope of the line).
* b is the bias (y-intercept).

To minimize the Mean Squared Error (MSE), the algorithm calculates the partial derivatives of the cost function and updates the parameters using a learning rate ($\alpha$):
w = w - \alpha \cdot \frac{1}{m} \sum_{i=1}^{m} (y_{pred}^{(i)} - y^{(i)}) \cdot x^{(i)}$$
b = b - \alpha \cdot \frac{1}{m} \sum_{i=1}^{m} (y_{pred}^{(i)} - y^{(i)})$$

## 🛠️ Prerequisites
To compile and run this project, you will need a standard C++ compiler (like GCC or Clang).

## 💻 Getting Started

1. **Clone the repository:**
   ```bash
   https://github.com/clived27/Linear-Regression-C-/

2. Compile the code:
   g++ -o regression main.cpp

3. Run the executable:
  ./regression


SAMPLE OUTPUT

Iteration = 0 | w = 4.312 | b = 0.814
Iteration = 1000 | w = 5.891 | b = 1.021
Converged early at iteration: 1452
Estimated Price of Plot with 2500 Sq.Feet is 14250000 Rupees
 
