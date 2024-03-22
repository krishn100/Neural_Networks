# Neural_Networks

Overview:
This project aims to develop a binary classification model using deep learning techniques to predict the success of startup funding applications received by Alphabet Soup, a venture capital firm. The dataset contains information about over 34,000 organizations that have received funding from Alphabet Soup, including whether or not they ultimately became successful.

Steps:

Data Preparation:
- Read the dataset (applicants_data.csv) into a Pandas DataFrame.
- Drop irrelevant columns (EIN and NAME).
- Encode categorical variables using OneHotEncoder.
- Concatenate numerical and encoded categorical variables into a single DataFrame.
- Split the data into features (X) and target (y) datasets.
- Scale the features using StandardScaler.

Model Building and Evaluation:
- Create a deep neural network model using TensorFlow's Keras.
- Compile the model with binary_crossentropy loss, adam optimizer, and accuracy metric.
- Fit the model with training data and evaluate it with test data.
- Save the model to an HDF5 file (AlphabetSoup.h5).

Model Optimization:
- Define and train three alternative models, adjusting various parameters such as the number of layers, neurons, activation functions, and epochs.
- Evaluate the performance of each alternative model in terms of loss and accuracy.
- Save each alternative model to HDF5 files for future use.

Results:

Model 1:
Loss: 0.634
Accuracy: 0.722
Model 2:
Loss: 0.625
Accuracy: 0.723
Model 3:
Loss: 0.691
Accuracy: 0.714

Conclusion:
While Model 2 demonstrated the best performance among the three models with the lowest loss and highest accuracy, further optimizations may be explored to improve the predictive capability of the model. 