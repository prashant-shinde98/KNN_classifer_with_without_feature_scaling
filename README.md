# K-Nearest Neighbors Classifier on Social Network Ads Dataset
This project implements a K-Nearest Neighbors (KNN) classifier to predict whether a user will purchase a product based on their age, gender, and estimated salary. The dataset used is the Social Network Ads dataset.

## Project Structure
Social_Net_class.csv: The dataset used for training and evaluation.

## Requirements
To run this project, you need the following Python packages:
-pandas
-scikit-learn
-matplotlib
-seaborn

## Dataset Description
The dataset includes the following columns:

- User ID: Unique identifier (dropped during preprocessing).
- Gender: Gender of the user (encoded as 0 or 1).
- Age: Age of the user.
- EstimatedSalary: Estimated salary of the user.
- Purchased: Target variable, where 1 indicates a purchase and 0 indicates no purchase.

## Steps
- Data Preprocessing
- Load the data and drop the User ID column.
- Encode the Gender column using LabelEncoder.
- Split the data into training and testing sets.
- Model Training

- Train a KNN classifier without feature scaling.
- Evaluate the model’s accuracy and confusion matrix.
- Apply feature scaling to the data and train a KNN classifier again.
- Evaluate the model with scaled features.

## Results
Model	Accuracy	Confusion Matrix
- Without Scaling	~81.7%	[[69, 4], [18, 29]]
- With Feature Scaling	~91.7%	[[68, 5], [5, 42]]
