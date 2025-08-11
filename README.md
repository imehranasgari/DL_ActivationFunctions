# Activation Functions & Derivatives — Hands-On Visualization

> A compact but purposeful notebook demonstrating my understanding of **activation function mechanics** and **gradients** in deep learning — with manual implementation, derivative computation, and visual comparison.

---

## 1) Project Title

**Visualization of Activation Functions and Their Derivatives**

---

## 2) Problem Statement and Goal of Project

A deep understanding of **activation functions** and their **derivatives** is essential for designing and debugging neural networks.
The goals of this project are to:

* Implement common activation functions and their derivatives **from scratch**.
* Plot and visually compare their behavior and gradients across a defined input range.
* Document intuitive insights into issues such as **vanishing gradients** and **dying ReLU**.

---

## 3) Solution Approach

* **Manual Implementation with NumPy** – all functions and derivatives are coded manually for transparency.
* **Functions Covered** (from the code): `sigmoid`, `tanh`, `relu`, `elu`, `selu`
* **Derivatives Implemented** for each activation (e.g., `sigmoid_derivative`, `relu_derivative`, etc.).
* **Parameters (as in the code)**:

  * `alpha = 1.0` for ELU
  * `lambda_ = 1.05070098` for SELU
* **Input Range**: `np.linspace(-10, 10, 100)`
* **Visualization**: Matplotlib plots of each activation function and its derivative over the same range.

---

## 4) Technologies & Libraries

* Python 3.x
* `numpy`
* `matplotlib`

---

## 5) Description about Dataset

**Not applicable** – This project is purely mathematical and does not use any dataset.

---

## 6) Installation & Execution Guide

**Install**

```bash
pip install numpy matplotlib
```

**Run**

1. Open `project.ipynb` in Jupyter Notebook or JupyterLab.
2. Execute cells sequentially to generate all activation and derivative plots.

> The notebook only requires NumPy and Matplotlib — no external files or pretrained weights.

---

## 7) Key Results / Performance

* **Main Output**: Clear plots showing each activation function and its gradient.
* Insights from the notebook’s visualizations:

  * **Sigmoid**: Saturates at extremes ⇒ very small gradients (vanishing).
  * **ReLU**: Simple and effective for positive inputs, but zero gradient for negative inputs ⇒ potential **dying ReLU**.
  * **ELU/SELU**: Smoother negative side with non-zero gradients ⇒ better gradient flow than ReLU.
  * **Tanh**: Centered output and stronger gradients near zero, but still saturates at extremes.

---

## 8) Screenshots / Sample Output

* All activation and derivative plots are produced inside the notebook (`matplotlib` outputs).
* Examples include:

  * `sigmoid` vs. `sigmoid_derivative`
  * `relu` vs. `relu_derivative`
  * `elu` vs. `elu_derivative`
  * `selu` vs. `selu_derivative`
  * `tanh` vs. `tanh_derivative`
    over the range `[-10, 10]`.

---

## 9) Additional Learnings / Reflections

* **From Mechanics to Intuition**: Writing the functions and derivatives manually deepened my intuition about gradient flow and saturation/zero zones.
* **Engineering Choices**: Choosing between ReLU, ELU, and SELU can be better justified by looking at their negative-side gradients.
* **Next Steps (if extended)**:

  * Add input normalization/noise and compare gradient responses.
  * Create a small Dense-layer experiment to compare convergence speeds with different activations.

---

## 👤 Author

**Mehran Asgari**
**Email:** [imehranasgari@gmail.com](mailto:imehranasgari@gmail.com)
**GitHub:** [https://github.com/imehranasgari](https://github.com/imehranasgari)

---

## 📄 License

This project is licensed under the **MIT License** – see the `LICENSE` file for details.

---

> 💡 *Some interactive outputs (e.g., plots, widgets) may not display correctly on GitHub. If so, please view this notebook via [nbviewer.org](https://nbviewer.org) for full rendering.*

---

