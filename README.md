# Vanishing_gradients_in_simple_RNNS
# Visualizing Vanishing Gradients in Simple RNNs from Scratch

## 📌 Introduction
Recurrent Neural Networks (RNNs) are powerful for sequential data but suffer from the **vanishing gradient problem**. This repository demonstrates how gradients diminish over time in a simple RNN, leading to ineffective learning. 

We implement an RNN **from scratch using TensorFlow** and visualize how gradients become too small for effective weight updates, highlighting why architectures like **LSTMs** and **GRUs** are needed.

## ⚙️ Implementation Details
- A **basic RNN** using only matrix multiplications and activation functions.
- **Categorical cross-entropy loss** for multi-class classification.
- **Adam optimizer** for training.
- **Gradient tracking** to visualize vanishing gradients.

##  Key Observations
- **Gradients shrink over time**, leading to almost no updates after multiple time steps.
- **Loss remains stagnant** despite training.
- **Tanh activation** worsens the issue as outputs saturate between -1 and 1.

##  Visualization
We track gradient magnitudes over epochs and show how they progressively shrink.



## 🛠️ Possible Fixes
To mitigate vanishing gradients:
1. **Use ReLU instead of Tanh**: Prevents extreme gradient shrinking.
2. **Use LSTMs or GRUs**: These architectures solve long-term dependency issues.


##  References
- Bengio, Y., Simard, P., & Frasconi, P. (1994). Learning long-term dependencies with gradient descent is difficult. *IEEE Transactions on Neural Networks*.



