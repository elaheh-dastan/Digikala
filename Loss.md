# MSE
It penalizes larger errors more heavily because of the squaring.

Sensitive to outliers

# MAE
- More robust to outliers than MSE.
- Has the same unit as the target variable (makes interpretation easier).

# R² Score (Coefficient of Determination)
R² tells you how much of the variance in the target variable is explained by your model.

![images/r2.png](images/r2.png)

Interpretation

- 𝑅2=1: perfect predictions
- 𝑅2=0: model predicts no better than the mean
- 𝑅2<0: model is worse than predicting the mean

# Cross Entropy
Used for:
→ Classification tasks (predicting discrete categories like “electronics”, “clothing”, etc.)

What it measures:
→ How far the predicted probability distribution is from the true class distribution.

yi: one-hot true label

Where it’s used:

- Classification (softmax output)
- Contrastive learning (after computing similarities + scaling + softmax)

Key property:

It’s sensitive to probabilities, not raw vector similarity.

# Cosine Similarity
What it measures:

→ The angle between two vectors — not their magnitude.

Key property:

It’s a distance metric, not a loss function by itself.

# logit scale


