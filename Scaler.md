# Robust Scaler
RobustScaler scales numerical features to reduce the influence of outliers. Unlike StandardScaler (which uses mean and standard deviation), it uses median and interquartile range (IQR)

When to use:

- When your data has outliers or heavy-tailed distributions.
- Especially for models sensitive to feature scale (e.g., KNN, SVM, gradient descent–based methods).
