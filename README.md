# Breast-Cancer-Classification-Using-Neural-Networks 🎗️
This project uses neural networks to classify breast cancer as malignant (cancerous) or benign (noncancerous). The dataset used for this project is the breast cancer Wisconsin (Diagnostic) dataset from the University of Wisconsin Hospitals. The data is collected by performing fine needle aspiration (FNA) on breast masses and then performing tests on the samples to determine whether the mass is cancerous or not.

**Dependencies**

The following libraries are used in this project: 📚

**numpy**: for numerical computing 🧮

**pandas**: for data processing and manipulation 🐼

**sklearn**: for machine learning and data preprocessing 📝

**tensorflow**: for building and training neural networks 🧠

**keras**: for building and training neural networks 🧠

**Data Collection and Processing** 📄🔃

The dataset is loaded using the **load_breast_cancer** function from **sklearn.datasets** library. The data is then loaded into a pandas dataframe and processed to add a target column indicating whether the tumor is malignant or benign.

The dataset contains 569 samples and 30 features. There are no missing values in the dataset. The label column contains the target variable, where 0 indicates ***malignant*** and 1 indicates ***Benign***.

**Data Splitting** 📑

The data is split into training data and testing data using the **train_test_split** function from **sklearn.model_selection** library. The test size is set to 20% of the data and the random state is set to 2.

**Data Standardization** 

The training and testing data are standardized using the **StandardScaler** function from **sklearn.preprocessing** library. The data is standardized to have zero mean and unit variance.

**Neural Network Architecture** 🧠🔍🔨

The neural network architecture consists of 2 hidden layers with 20 neurons each and an output layer with 2 neurons (one for each class). The activation function used for the hidden layers is **ReLU** and the output layer uses **sigmoid activation**.

The loss function used for the model is **sparse_categorical_crossentropy** and the optimizer used is **adam**. The model is trained for 10 epochs with a validation split of 0.1.

**Predictive System** 🔮

The predictive system takes input data in the form of a tuple containing the 30 features of a breast mass. The data is then standardized and fed into the trained model to predict whether the mass is malignant or benign.
