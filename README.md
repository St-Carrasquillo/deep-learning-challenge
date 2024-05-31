# deep-learning-challenge
Module 21 Neural Networks and Deep Learning

## Data Preprocessing
- **Loaded Data**: The dataset containing information about organizations that received funding from Alphabet Soup.
- **Dropped Columns**: The non-beneficial columns `EIN` and `NAME` were dropped.
- **Categorical Encoding**: The `APPLICATION_TYPE` and `CLASSIFICATION` columns were examined and less frequent categories were replaced with "Other". All categorical data were then converted to numeric using `pd.get_dummies`.
- **Feature and Target Split**: The preprocessed data was split into feature (`X`) and target (`y`) arrays.
- **Data Splitting**: The data was split into training and testing sets.

## Model Building and Training
- **Scaling**: The feature data was scaled using `StandardScaler`.
- **Model Architecture**:
  - A deep neural network with two hidden layers:
    - First hidden layer: 80 nodes, ReLU activation
    - Second hidden layer: 30 nodes, ReLU activation
    - Output layer: 1 node, Sigmoid activation
- **Compilation**: The model was compiled with `binary_crossentropy` loss, `adam` optimizer, and `accuracy` metric.
- **Training**: The model was trained for 100 epochs.

## Model Evaluation
- The model achieved an accuracy of approximately 72.65% on the test data.

## Results
- **Loss**: 0.5696
- **Accuracy**: 0.7265

## Model Export
- The trained model was saved in the HDF5 format and because of a suggestion when running in colab saved in the Keras format as `AlphabetSoupCharity`.



