## 1. Overview

This assignment transforms the NO2 feature using a roll‑number–based nonlinear function and fits a probability density function (PDF):
p(z) = c * exp( -lambda * (z - mu)^2 )
You must compute the parameters lambda, mu, and c and compare the predicted PDF with the transformed data distribution.

---

## 2. Methodology 

### Step 1 — Load Data

* Extract NO2 feature.
* Handle missing values.

### Step 2 — Apply Roll‑Number Transformation

Formula:
z = x + a_r * sin(b_r * x)
Where:

* a_r = 0.05 * (r mod 7)
* b_r = 0.3 * (r mod 5 + 1)
* r = your roll number

### Step 3 — Fit the PDF

Estimate lambda, mu, c using optimization functions such as curve_fit or likelihood minimization.

### Step 4 — Visualization

* Plot histogram of transformed z.
* Overlay the fitted PDF curve.

---

## 3. Results

### Parameter Table

(Insert your actual values)

| Parameter | Estimated Value |
| --------- | --------------- |
| lambda    | value           |
| mu        | value           |
| c         | value           |

### Graph Interpretation

* Histogram shows the empirical shape of transformed z.
* PDF curve shows the fitted model.
* Close alignment means good parameter estimation.

---

## 4. Key Takeaways

* Transformation adds nonlinearity to the feature.
* The fitted PDF approximates the new distribution.
* Parameters reflect spread (lambda), center (mu), and scale (c).

---

## 5. Files Included

* 102317269_Ass3.ipynb — main code.
* README.md — documentation.

---

## 6. Conclusion

The assignment demonstrates nonlinear transformation, PDF fitting, optimization, and visualization in a compact workflow.
