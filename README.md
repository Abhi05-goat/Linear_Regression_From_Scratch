# Linear Regression from Scratch

## Overview

This repository contains an implementation of **Linear Regression** using **Gradient Descent** from scratch. The model is trained on a dataset that maps **years of experience** to **salary**, learning a regression line to predict salaries based on experience.

## Features

- Loads a **real-world salary dataset** (`Salary_dataset.csv`).
- **Implements Linear Regression** from scratch using **Gradient Descent**.
- Calculates **Mean Squared Error (MSE) loss function**.
- Visualizes the **dataset, regression line, and cost function evolution**.
- Allows modification of **hyperparameters** such as learning rate and number of epochs.

## Dataset

The dataset contains two key columns:
- **YearsExperience**: Number of years of experience.
- **Salary**: Corresponding salary for that experience.

## Model Implementation

### Loss Function
The loss function used is **Mean Squared Error (MSE)**:
```math
L(w, b) = \frac{1}{2n} \sum_{i=1}^{n} (y_i - (w x_i + b))^2
```
Where:
- **w**: Weight (slope of the regression line)
- **b**: Bias (intercept)
- **x**: Years of experience
- **y**: Salary
- **n**: Number of samples

### Training Algorithm
1. Initialize **weight (w) and bias (b) to zero**.
2. Iterate over **epochs**:
   - Compute **MSE loss**.
   - Compute **gradients** for w and b.
   - Update w and b using **Gradient Descent**.
3. Train until convergence.

## Dependencies
To run this project, install the required libraries:
```bash
pip install numpy pandas matplotlib
```

## Usage
Clone the repository and run the script:
```bash
git clone https://github.com/Abhi05-goat/linear-regression.git
cd linear-regression
python linear_regression.py
```

## Visualization
The script generates the following visualizations:
1. **Scatter Plot of Data** (Years of Experience vs Salary).
2. **Regression Line** fitted on the dataset.
3. **Cost Function vs Weight** plot.
4. **Cost Function vs Bias** plot.

---

### 1. Scatter Plot of Data
![image](https://github.com/user-attachments/assets/e1ee5071-6432-4ead-b8ba-70813193328c)

### 2. Regression Line
![image](https://github.com/user-attachments/assets/b228eb15-7ef2-4c10-9de6-9a5811f5f07e)

### 3. Cost vs Weight
![image](https://github.com/user-attachments/assets/55a1c2b5-7ee6-4491-87e8-902a9b9e5ba0)

### 4. Cost vs Bias
![image](https://github.com/user-attachments/assets/8ba2b8aa-cebd-4d72-90b8-330303933f07)

---

## Hyperparameters
Modify the hyperparameters in the script:
```python
learning_rate = 0.0001  # Step size for gradient descent
epochs = 1000  # Number of training iterations
```

## Results
- The model successfully learns a **linear relationship** between experience and salary.
- Gradient Descent optimizes the weights and bias to minimize error.
- The trained model can predict salaries based on years of experience.

## Author
[Abhivanth] - [https://github.com/Abhi05-goat]

## License
This project is licensed under the **MIT License**. See `LICENSE` for details.

Feel free to contribute by submitting pull requests or reporting issues!

