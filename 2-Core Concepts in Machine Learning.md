 **Core Concepts in Machine Learning**

 **1\. Features and Labels**  
   *\- Definition:*  
     \- Features: Input data variables that describe the characteristics of an instance.  
     \- Labels: The output or target variable that you want to predict.

   *\- Real-Life Example:* Predicting house prices.  
     \- Features: Size (square feet), number of bedrooms, location.  
     \- Label: The actual price of the house.

   *\- Use Case:* A real estate agency uses historical data to predict future house prices based on various features.

<img width="640" alt="1708280037789" src="https://github.com/user-attachments/assets/b1e20e97-c926-4f5f-8298-dacfe7c0e032">

 **2\. Training, Validation, and Test Sets**  
   *\- Definition:*  
     \- Training Set: Data used to train the model.  
     \- Validation Set: Data used to tune the model's hyperparameters and avoid overfitting.  
     \- Test Set: Data used to evaluate the model's performance on new, unseen data.

   *\- Real-Life Example:* Email spam detection.  
     \- Training Set: A dataset of emails with known labels (“Spam” or “Not Spam”).  
     \- Validation Set: A smaller set of emails used to adjust the model's parameters.  
     \- Test Set: A set of new emails to assess how well the model identifies spam.

   *\- Use Case:* An email service uses a machine learning model to classify incoming messages as spam or not based on the words and phrases in emails.  

   ![10994_2022_6176_Fig5_HTML](https://github.com/user-attachments/assets/46ece7f0-6b61-4386-9047-7c8596decfa3)
   
   \- Formula (Splitting Data):  
     \- Training Data \= 70%  
     \- Validation Data \= 15%  
     \- Test Data \= 15%

 **3\. Overfitting vs. Underfitting**  
   *\- Definition:*  
     \- Overfitting: When the model learns the training data too well, including noise, and performs poorly on new data.  
     \- Underfitting: When the model is too simple to capture the underlying patterns in the data.

   *\- Real-Life Example:* Predicting stock prices.  
     \- Overfitting: The model matches the stock data history perfectly but fails to predict future prices accurately.  
     \- Underfitting: The model predicts that prices will always stay the same, missing important trends.  
   *\- Use Case:* A financial analyst uses a model to forecast stock prices. They aim for a balance to avoid overfitting (capturing daily fluctuations) and underfitting (missing key market trends).  

   ![download](https://github.com/user-attachments/assets/01cb790e-41a7-41d5-b979-57ecd2bedddf)
   
   \- Formula (Model Complexity):  
     \- Overfitting occurs when the model complexity (M) is too high:  
       \- M\_complex → Overfitting  
     \- Underfitting occurs when the model complexity (M\_simple) is too low:  
       \- M\_simple → Underfitting  
     \- M\_simple: Represents a model that is not complex enough to capture patterns in the data. For example, using a straight line (linear regression) to model a complex curve.

 **4\. Bias-Variance Tradeoff**  
   *\- Definition:*  
     \- Bias: Error due to the model's assumptions (e.g., linear models for non-linear data). High bias means the model is too simple.  
     \- Variance: Error due to the model's sensitivity to fluctuations in the training data. High variance means the model is too complex.  
     \- Tradeoff: A balance between a model that is too simple (high bias, low variance) and one that is too complex (low bias, high variance).

   *\- Real-Life Example:* Diagnosing a disease based on patient symptoms.  
     \- High Bias: Using a simple model like "all patients are healthy" results in missed diagnoses.  
     \- High Variance: Using a complex model that changes significantly with each new patient's data may misdiagnose due to small variations.

   *\- Use Case:* A hospital uses a model to predict the likelihood of a disease based on symptoms, trying to ensure the model isn't overly complex or overly simple.  
   
   ![1_RQ6ICt_FBSx6mkAsGVwx8g](https://github.com/user-attachments/assets/888fdc2c-b8bd-4788-be07-abec08145d2e)
   
   \- Formula (Mean Squared Error Decomposition):  
                                MSE \= Bias^2 \+ Variance \+ Irreducible Error

* MSE (Mean Squared Error): A measure of how well the model predicts outcomes.  
* Bias: Measures how far the predictions are from actual values.  
* Variance: Measures how predictions vary with changes in the training data.  
* Irreducible Error: Error that is inherent in the data and cannot be reduced.

