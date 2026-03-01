# Quick Start

This guide explains how to quickly run and understand the **Normal Equations solver (scalar form)** for simple linear regression.

---

## 🚀 1. Clone the Repository

```bash
git clone https://github.com/USERNAME/Normal-equations-scalar-form-solver-course.git
cd Normal-equations-scalar-form-solver-course
````

---

## 🧠 2. Mathematical Background

We solve the simple linear regression problem:

$$
y_i = \beta_0 + \beta_1 x_i + \varepsilon_i
$$

in least squares form:

$$
\min_{\beta_0, \beta_1} \sum_{i=1}^{n} (y_i - \beta_0 - \beta_1 x_i)^2
$$

---

## 🔎 3. Closed-Form Solution

Using the normal equations:

$$
(X^T X)\beta = X^T y
$$

The solution is:

$$
\beta = (X^T X)^{-1} X^T y
$$

For scalar regression, the slope and intercept can be written explicitly:

$$
\hat{\beta}_1 =
\frac{\sum (x_i - \bar{x})(y_i - \bar{y})}
{\sum (x_i - \bar{x})^2}
$$

$$
\hat{\beta}_0 = \bar{y} - \hat{\beta}_1 \bar{x}
$$

---

## 💻 4. Run the Solver

Install dependencies:

```bash
pip install -r requirements.txt
```

Run the example:

```bash
python example.py
```

Or import the solver in Python:

```python
from solver import normal_equation_scalar

beta0, beta1 = normal_equation_scalar(x, y)

print(beta0, beta1)
```

---

## 📊 5. Visualization (If Included)

If the project contains visualization:

```bash
python visualize.py
```

You should see:

* Data points
* Regression line
* Fitted model

---

## 🧪 6. Run Tests

If tests are included:

```bash
pytest
```

---

## 🎯 What You Learned

After running this project, you understand:

✔ How normal equations are derived
✔ How closed-form least squares works
✔ Why matrix inversion appears
✔ How scalar form relates to matrix form

---
