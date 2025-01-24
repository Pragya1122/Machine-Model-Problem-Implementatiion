# Machine-Model-Problem-Implementatiion


*Company* : CODETECH IT SOLUTIONS

*Name* : PRAGYA SANTRA

*Intern ID* : CT08NGE

*Domain* : Python

*Duration* : 4 Weeks

*Mentor* : NEELA SANTOSH


## Description


In this task, the goal is to create a predictive machine learning model that classifies or predicts outcomes from a dataset using **Scikit-learn**. A typical example of such a task is **spam email detection**, where the objective is to predict whether an email is spam or not based on its content. This task involves several key stages: data loading, exploration, preprocessing, model selection, training, evaluation, and fine-tuning. The process showcases how machine learning can be applied to a real-world problem, such as filtering out unwanted emails.

The first step in building the spam detection model is to **load the dataset**. For this example, we used a CSV file called `spam_ham_dataset.csv`, which consists of labeled data containing emails and their respective labels, indicating whether they are "spam" or "ham" (non-spam). After loading the data into a Pandas DataFrame, an essential step is to **explore the dataset**. This involves checking for any missing values, inspecting the column types, and analyzing the distribution of labels to understand how balanced the dataset is. For spam email detection, it is important to note whether the dataset has an equal or skewed distribution of spam and ham emails.

Once the dataset is loaded and explored, the next crucial step is **data preprocessing**. Since the task involves text data, we use the **TF-IDF (Term Frequency-Inverse Document Frequency)** vectorizer to convert the textual data into numerical features. TF-IDF is commonly used for text classification tasks because it converts text into vectors that capture the importance of words in documents. This transformation allows the machine learning model to learn from the text data. Additionally, the labels for spam and ham emails need to be encoded numerically. In this case, we used **LabelEncoder** from Scikit-learn to convert the categorical labels into binary numerical values, with 0 representing ham and 1 representing spam.

Once the data is preprocessed, it is split into **training and testing sets** using **train_test_split**. This is done to ensure that the model is trained on one subset of the data and evaluated on another, unseen subset to check its generalization ability. In this example, the dataset is split into 80% for training and 20% for testing. After splitting the data, the next step is to **train the machine learning model**. In this case, we used **Logistic Regression**, which is a simple yet effective model for binary classification tasks such as spam detection. Logistic Regression works by estimating the probability that an input belongs to a particular class, and in this case, it learns to differentiate between spam and non-spam emails.

After training the model, the next step is to **evaluate its performance**. Evaluation is crucial to understanding how well the model generalizes to unseen data. We use several metrics, including **accuracy**, **confusion matrix**, and **classification report**. Accuracy provides an overall measure of how many predictions were correct. The confusion matrix, on the other hand, breaks down the true positives, true negatives, false positives, and false negatives, helping to evaluate the model’s performance more comprehensively. The classification report includes additional metrics such as precision, recall, and F1-score, which are particularly important in imbalanced datasets, like spam detection, where one class (ham) might be more frequent than the other (spam).

To further improve the model, **hyperparameter tuning** can be performed using **GridSearchCV**. Hyperparameter tuning allows for selecting the best parameters for the model, which can help improve performance. For Logistic Regression, this might include adjusting the regularization strength or solver used during optimization. By using GridSearchCV, we can find the combination of hyperparameters that yields the best model performance.


### Screenshot of the output

![Image](https://github.com/user-attachments/assets/3f983722-7dc8-4e4f-bd92-ba58a05e6cdb)


![Image](https://github.com/user-attachments/assets/2a3c4cf3-a6f2-42b4-b72c-21f9f0473a3f)


![Image](https://github.com/user-attachments/assets/ee2d9612-d998-4694-b814-0e66408b796f)


![Image](https://github.com/user-attachments/assets/5d131beb-5a75-46bf-a720-0b33070457e7)


![Image](https://github.com/user-attachments/assets/cfbeb8fe-4a9b-4cbe-b06e-03a49b827e54)
