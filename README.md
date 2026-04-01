### **Project Overview**
This project evaluates three deep learning architectures **Deep Neural Networks (DNN)**, **Convolutional Neural Networks (CNN)**, and **Long Short-Term Memory (LSTM)** to predict which customers are likely to leave a bank. It specifically addresses the challenge of **class imbalance**, where churned customers are a minority in the dataset.

### **1. Data Preprocessing & Balancing**
* **Feature Engineering:** New features were created (e.g., `RiskScore`, `Age_Balance`) to better capture behavioral patterns.
* **Handling Skewness:** Logarithmic transformations were applied to skewed numerical features.
* **Class Balancing:** The **SMOTETomek** technique was used to balance the dataset, ensuring the models could effectively learn from both churned and non-churned classes.

### **2. Deep Learning Architectures**
* **DNN:** A multilayer feedforward network used to capture global feature interactions.
* **CNN:** Utilized 1D convolutional layers to extract local feature patterns from the tabular data.
* **LSTM:** Though typically for sequential data, the LSTM was creatively used to treat feature vectors as sequences to learn order-dependent representations.

### **3. Model Tuning & Optimization**
* **Hyperparameter Tuning:** Random Search and Keras Tuner were implemented to optimize activation functions, optimizers (Adam, Nadam, RMSprop), and dropout rates.
* **Regularization:** Batch Normalization, Dropout, and L2 regularization were used to prevent overfitting and ensure the models generalize well to new data.

### **4. Key Results**
* **Top Performer:** The **LSTM model** (Experiment 3) emerged as the best overall, achieving a test accuracy of **88.88%** and an AUC of **0.96**.
* **Evaluation Metrics:** Beyond accuracy, the project focused on precision, recall, and F1-score to ensure the minority churn class was accurately detected.

### **Summary of the Repository**
The code provides a complete end-to-end pipeline: from **Exploratory Data Analysis (EDA)** and advanced **balancing techniques** to implementing and **tuning deep learning models** for financial risk prediction.
