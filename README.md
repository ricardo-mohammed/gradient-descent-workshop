# Workshop: Gradient Descent in Single- and Multi-Layer Neural Networks

**Course:** Foundations of Machine Learning Frameworks
**Team members:**

- Ricardo Mohammed — 7500382
- Juan Camilo Chirivi — 9115141
- Zeynep Ozdemir — 9045142
- Senay Teweldebrhan — 9120588

**Submission date:** November 27th, 2026
**Repository:** [GradientDescent_Workshop](https://github.com/ricardo-mohammed/GradientDescent_Workshop.git)

## Setup

Use Python 3.14.5 to create and activate a virtual environment, then install the project requirements:

```powershell
py -3.14 -m venv .venv
.venv\Scripts\Activate.ps1
python --version
python -m pip install -r requirements.txt
```

Confirm that `python --version` reports Python 3.14.5. In VS Code, open `notebooks/GradientDescent_Workshop.ipynb` and select the `.venv` environment as the notebook kernel. Run the notebook from top to bottom.

## Workshop overview

The workshop develops gradient descent from its mathematical intuition to neural-network training. It introduces loss functions, gradients, negative-gradient updates, and learning rates, then applies these ideas to a single parameter, a neuron, and multi-layer networks. It also compares batch, stochastic, and mini-batch gradient descent and explains how backpropagation efficiently computes gradients.

The practical sections use PyTorch to inspect tensors and gradients, perform manual updates, fit a linear model, and train a small multi-layer network. The challenges extend the training workflow to PyTorch autograd, TensorFlow's `GradientTape`, and Keras's built-in and custom training APIs.

## Section 17: Reflection challenge

- **17(A) — Conceptual understanding:** Explain what the gradient tells us, why gradient descent moves in the negative-gradient direction, how the learning rate affects updates, why optimization is iterative, and why multi-layer networks use backpropagation.
- **17(B) — Practical understanding:** Consider the effects of very small gradients and overly large learning rates, why mini-batches are widely used, and why PyTorch gradients must be reset between iterations.
- **17(C) — Framework comparison:** Compare how PyTorch, TensorFlow, and Keras calculate gradients and perform updates, including the convenience and flexibility of Keras's `model.fit()`.
- **17(D) — Synthesis:** Describe gradient descent both intuitively, without equations, and mathematically using a local linear approximation.
