# Position Salary Prediction using SVR (Support Vector Regression)

This project implements a machine learning model using Support Vector Regression (SVR) to predict salaries based on position levels. It demonstrates how to preprocess data, apply feature scaling, train an SVR model with an RBF kernel, and visualize the results with both standard and high-resolution plots.

---

## 📁 Dataset

The dataset used is `Position_Salaries.csv`, which contains:

- **Position Title** (ignored in this script)
- **Level** (numerical value representing position level)
- **Salary** (target value to be predicted)

Example:

| Position       | Level | Salary     |
|----------------|-------|------------|
| Business Analyst | 1   | 45000      |
| CEO            | 10    | 1000000    |

---

## 🚀 Workflow

1. **Import Libraries**  
   Uses `NumPy`, `Pandas`, `Matplotlib`, and `scikit-learn`.

2. **Load Dataset**  
   Loads the position levels (`X`) and salaries (`y`).

3. **Reshape Target**  
   Reshapes `y` into a 2D array for scaling compatibility.

4. **Feature Scaling**  
   Applies standardization using `StandardScaler` to both `X` and `y`.

5. **Train Model**  
   Trains an SVR model with an RBF (Radial Basis Function) kernel.

6. **Predict New Value**  
   Predicts the salary for a position level of 6.5 after inverse transforming the scaled result.

7. **Visualize Results**  
   - **Basic Plot**: Shows model predictions over original data points.
   - **High-Resolution Plot**: Smooth curve by evaluating the model on a fine-grained range of input values.

---

## 📈 Example Output

- Red dots represent actual salaries.
- Blue curve shows the model's predictions.
- The high-res plot provides a smoother visualization of the SVR model's behavior.

---

## 🛠️ Requirements

- Python 3.x
- pandas
- numpy
- matplotlib
- scikit-learn

Install dependencies:

```bash
pip install numpy pandas matplotlib scikit-learn
