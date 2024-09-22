###KNN ALGORITHM
The **K-Nearest Neighbors (KNN)** algorithm is a simple and intuitive **supervised machine learning** algorithm used for **classification** and **regression** tasks. Here's a brief overview:

### How KNN Works:
1. **Training Phase**: 
   - KNN does not have a separate training phase. Instead, it memorizes the dataset, making it a **lazy learning algorithm**.

2. **Prediction Phase**:
   - For a new data point, the algorithm finds the **K nearest neighbors** (based on a distance metric like **Euclidean distance**).
   - The most common classes among the neighbors (for classification) or the average value (for regression) is used to predict the output.
   
### Key Steps:
1. **Choose K**: Select the number of neighbors (**K**). Common choices include odd numbers (e.g., 3, 5) to avoid ties in classification.
2. **Calculate Distance**: Compute the distance between the new point and all points in the training dataset (often using Euclidean distance, but other metrics like Manhattan distance can be used).
3. **Select Neighbors**: Identify the **K nearest points**.
4. **Majority Vote**: In classification, the most frequent class label among the K neighbors determines the predicted class.

### Distance Metrics:
- **Euclidean Distance**: Commonly used for continuous variables, calculated as the straight-line distance between two points.
- **Manhattan Distance**: Useful when dealing with grid-like data.
  
### Advantages:
- **Simple to implement** and intuitive.
- **No training phase**: The model just memorizes the data.
- **Flexible**: Works for both classification and regression.

### Disadvantages:
- **Computationally expensive** during prediction, as it involves calculating the distance to every point in the dataset.
- **Sensitive to noise**: Outliers or irrelevant features can affect accuracy.
- **Curse of dimensionality**: Performance decreases in high-dimensional spaces.

### Use Cases:
- **Image Recognition**
- **Recommendation Systems**
- **Text Categorization**
