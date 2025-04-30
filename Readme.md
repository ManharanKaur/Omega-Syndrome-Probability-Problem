# Omega Syndrome Probability Problem

## Overview
This project analyzes the **Omega Syndrome**, a fictional medical condition, using **Bayesian probability** based on observed symptoms. It includes a dynamic **D3.js tree visualizer** that models the conditional paths to calculate the probability of having Omega Syndrome.

---

## Live Visualization

View the interactive Bayes Tree:
# [Problem Statement](./Bayes_ques.html)

---

##  Problem Description

Given:
- A prior probability: `P(Omega) = 0.001`
- Symptoms (Markers) with conditional probabilities:
  - `P(A | Omega) = 0.95`, `P(B | Omega) = 0.90`, `P(C | Omega) = 0.85`
  - `P(A | ¬Omega) = 0.10`, `P(B | ¬Omega) = 0.05`, `P(C | ¬Omega) = 0.02`

You must calculate the **posterior probability** that a patient has Omega Syndrome given all three symptoms A, B, and C are present.

---

##  Bayes’ Theorem

\[
P(Omega | A ∧ B ∧ C) = \frac{P(A ∧ B ∧ C | Omega) \cdot P(Omega)}{P(A ∧ B ∧ C)}
\]

Where:

- \( P(A ∧ B ∧ C | Omega) = P(A|Omega) \cdot P(B|Omega) \cdot P(C|Omega) \)
- \( P(A ∧ B ∧ C | \neg Omega) = P(A|¬Omega) \cdot P(B|¬Omega) \cdot P(C|¬Omega) \)
- Total probability:
\[
P(A ∧ B ∧ C) = P(A ∧ B ∧ C | Omega) \cdot P(Omega) + P(A ∧ B ∧ C | ¬Omega) \cdot P(¬Omega)
\]

---

##  Sample Output

Using the values above:
- Posterior probability of Omega Syndrome after observing all 3 markers = **~13.94%**

---

##  Features

- Interactive **D3.js Bayes Tree** to explore probability paths
- Real-time **tooltip probabilities** on each node
- Clearly visualized **Omega vs non-Omega** decision branches
- Posterior calculation based on selected symptoms


