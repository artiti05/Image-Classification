# CIFAR-10 Classification using Logistic Regression

## Overview
This project implements a logistic regression model to classify images from the CIFAR-10 dataset. The CIFAR-10 dataset consists of 60,000 images categorized into the following classes:

- Airplane
- Automobile
- Bird
- Cat
- Deer
- Dog
- Frog
- Horse
- Ship
- Truck

Each image is 32x32 pixels in RGB format. The logistic regression model is trained to predict the class of each image based on its features.

## Key Results

### Loss Curve
- **Description:** The loss curve plots the loss function value against the number of epochs during training.
- **Observations:**
  - The loss decreases steadily over 10 epochs, starting at approximately 1.675 and ending near 1.655.
  - This indicates that the model is learning, but the small decrease suggests that logistic regression has limitations when handling a complex dataset like CIFAR-10.

### Confusion Matrix
- **Description:** Compares the predicted class labels (horizontal axis) to the true class labels (vertical axis) for the CIFAR-10 test data.
- **Observations:**
  - Strong diagonal elements indicate correct classifications in classes like airplane, automobile, frog, and truck.
  - Misclassifications are observed, e.g., many ship images are misclassified as airplanes. Birds are often confused with cats and dogs due to visual similarities.
  - The confusion matrix highlights the model's challenges with certain classes.

### Accuracy Per Class
- **Description:** A bar chart shows the accuracy per class for the logistic regression model.
- **Observations:**
  - Highest accuracy (close to 50%) for ship and truck classes.
  - Lowest accuracy for bird and cat classes, suggesting difficulty in distinguishing these categories.
  - Intermediate performance for deer, dog, and horse classes (30-40% accuracy).
  - Airplane and automobile achieve above-average accuracy but still underperform compared to ship and truck.

### Prediction Examples
- **Predicted Labels (Pred):** The labels predicted by the model.
- **True Labels (True):** The actual class labels of the images.

## Insights
1. Logistic regression can provide a baseline performance for image classification tasks but struggles with the complexity of datasets like CIFAR-10.
2. Model optimization and data augmentation are needed to improve performance, particularly for underperforming classes like bird and cat.

## How to Run the Code
1. Install the required Python packages (numpy, pandas, matplotlib, etc.).
2. Load the `Logistic-Regression.ipynb` notebook.
3. Follow the steps in the notebook to preprocess the data, train the model, and visualize the results.
4. Review the plots and metrics, including the loss curve, confusion matrix, and accuracy per class, to evaluate the model's performance.

## Conclusion
This project highlights the challenges of using logistic regression for image classification and provides insights into the strengths and weaknesses of the model when applied to the CIFAR-10 dataset.
