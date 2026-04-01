### **Project Overview**
[cite_start]This project evaluates three deep learning architectures—**Deep Neural Networks (DNN)**, **Convolutional Neural Networks (CNN)**, and **Long Short-Term Memory (LSTM)**—to predict which customers are likely to leave a bank[cite: 4, 168]. [cite_start]It specifically addresses the challenge of **class imbalance**, where churned customers are a minority in the dataset[cite: 49, 1001].

### **1. Data Preprocessing & Balancing**
* [cite_start]**Feature Engineering:** New features were created (e.g., `RiskScore`, `Age_Balance`) to better capture behavioral patterns[cite: 195, 1184].
* [cite_start]**Handling Skewness:** Logarithmic transformations were applied to skewed numerical features[cite: 198, 1187].
* [cite_start]**Class Balancing:** The **SMOTETomek** technique was used to balance the dataset, ensuring the models could effectively learn from both churned and non-churned classes[cite: 41, 1200].

### **2. Deep Learning Architectures**
* [cite_start]**DNN:** A multilayer feedforward network used to capture global feature interactions[cite: 42, 1029].
* [cite_start]**CNN:** Utilized 1D convolutional layers to extract local feature patterns from the tabular data[cite: 100, 1064].
* [cite_start]**LSTM:** Though typically for sequential data, the LSTM was creatively used to treat feature vectors as sequences to learn order-dependent representations[cite: 126, 127].

### **3. Model Tuning & Optimization**
* [cite_start]**Hyperparameter Tuning:** Random Search and Keras Tuner were implemented to optimize activation functions, optimizers (Adam, Nadam, RMSprop), and dropout rates[cite: 6, 1438].
* [cite_start]**Regularization:** Batch Normalization, Dropout, and L2 regularization were used to prevent overfitting and ensure the models generalize well to new data[cite: 1307, 1376, 1385].

### **4. Key Results**
* [cite_start]**Top Performer:** The **LSTM model** (Experiment 3) emerged as the best overall, achieving a test accuracy of **88.88%** and an AUC of **0.96**[cite: 8, 1442, 1448].
* [cite_start]**Evaluation Metrics:** Beyond accuracy, the project focused on precision, recall, and F1-score to ensure the minority churn class was accurately detected[cite: 182, 1410].

### **Summary of the Repository**
[cite_start]The code provides a complete end-to-end pipeline: from **Exploratory Data Analysis (EDA)** and advanced **balancing techniques** to implementing and **tuning complex deep learning models** for financial risk prediction[cite: 1158, 1208].
