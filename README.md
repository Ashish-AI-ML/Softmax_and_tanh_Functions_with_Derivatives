# 📊 Softmax and tanh Functions with Derivatives – Visualization and Comparison

This project provides an interactive visualization and comparison of two fundamental activation functions in neural networks:

- **Softmax function** and its **derivatives (Jacobian diagonal)**
- **tanh function** and its **derivative**

It is designed to help deep learning practitioners and students understand how these functions behave and where to apply them effectively.

---

## 🔢 Softmax Function

### Formula
\[
\text{softmax}(x_i) = \frac{e^{x_i}}{\sum_j e^{x_j}}
\]

### Characteristics
- **Purpose**: Converts a vector of real numbers into a **probability distribution**.
- **Range**: \( (0, 1) \); all outputs sum to 1.
- **Common Use**: Final output layer for **multi-class classification** (e.g., image recognition, NLP).
- **Derivative**: Produces a **Jacobian matrix** used during backpropagation.

---

## 🔁 tanh Function

### Formula
\[
\tanh(x) = \frac{e^x - e^{-x}}{e^x + e^{-x}}
\]

### Characteristics
- **Purpose**: Produces **zero-centered** output.
- **Range**: \( (-1, 1) \)
- **Common Use**: **Hidden layers** in neural networks.
- **Derivative**:
  \[
  \tanh'(x) = 1 - \tanh^2(x)
  \]
- **Advantage**: More balanced gradient flow than sigmoid (less prone to saturation).

---

## 📈 Combined Visualization

This project includes plots for:

- **Softmax outputs** for a 3-element input vector as one element varies
- **Diagonal of the softmax Jacobian matrix** (partial derivatives)
- **tanh function** curve
- **Derivative of tanh**

### Comparison Goals
| Feature               | Softmax                   | tanh                      |
|-----------------------|---------------------------|---------------------------|
| **Output Range**      | (0, 1), sum = 1            | (-1, 1)                   |
| **Use Case**          | Final layer (classification) | Hidden layers            |
| **Non-linearity**     | Yes                       | Yes                       |
| **Derivative Shape**  | Depends on vector values   | Peaks at 0, symmetric     |
| **Problem Solving**   | Class probability          | Feature transformation    |

---

## 🛠️ How to Use

### Requirements
- `numpy`
- `matplotlib`

### Install Dependencies
```bash
pip install numpy matplotlib
