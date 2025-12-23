# MACHINE-LEARNING-MODEL-IMPLEMENTATION

## Spam Email Detection Using Scikit-Learn

__Company Name__ : Codtech IT Solutions Private Limited

__Name__ : Kiruthika R

__Intern ID__ : CTIS0400

__Domain Name__ : Python Programming.

__Duration__ : 4 weeks

__Mentor__ : Neela Santhosh Kumar  

<img width="830" height="524" alt="Image" src="https://github.com/user-attachments/assets/9d0851eb-ef4b-42ae-9623-2baf26f263f5" />

__1. Introduction__

With the rapid growth of digital communication, email has become one of the most widely used platforms for information exchange. However, the increase in email usage has also led to a significant rise in spam emails, which can be harmful, misleading, or time-consuming for users. Detecting spam emails automatically is an important application of machine learning classification techniques.

This project focuses on developing a predictive machine learning model using scikit-learn to classify emails as Spam or Not Spam (Ham). The model is trained on a labeled dataset and evaluated using standard performance metrics.

__2. Objective__

The primary objectives of this project are:

- To build a machine learning classification model using Python and scikit-learn.

- To preprocess and transform textual email data into numerical features.

- To train a model capable of accurately identifying spam emails.

- To evaluate the model using appropriate performance metrics.

- To demonstrate the practical application of machine learning in text classification.

__3. Dataset Description__

The dataset used in this project is the SMS Spam Collection Dataset, which contains a collection of labeled SMS messages.

➤ Total Instances: 5,572 messages.

➤ label: Indicates whether the message is spam or ham.

➤ message: The actual text content of the message.

The dataset is balanced enough to allow effective learning and is widely used for benchmarking spam detection algorithms.

__4. Methodology__

The project follows a standard machine learning pipeline, consisting of the following steps:

##### 4.1 Data Preprocessing :

Labels were converted into numeric format:

➤ Spam → 1

➤ Ham → 0

Text data was cleaned implicitly using vectorization techniques that remove stop words.

##### 4.2 Feature Extraction

Since machine learning models cannot directly process text, the TF-IDF (Term Frequency–Inverse Document Frequency) technique was used to convert textual data into numerical feature vectors. TF-IDF emphasizes important words while reducing the impact of commonly used terms.

##### 4.3 Train-Test Split

The dataset was split into:

➤ 75% Training data

➤ 25% Testing data

This ensures that the model is evaluated on unseen data to measure its generalization capability.

##### 4.4 Model Selection

The Multinomial Naive Bayes algorithm was selected because:

➤ It is computationally efficient.

➤ It performs well on text classification problems.

➤ It works effectively with TF-IDF features.

__5. Model Implementation__

The model was implemented using the scikit-learn library. The training process involved fitting the Naive Bayes classifier on the TF-IDF transformed training data. After training, the model was used to predict labels for the test dataset.

__6. Model Evaluation__

The performance of the model was evaluated using the following metrics:

##### 6.1 Accuracy

Accuracy measures the overall correctness of the model.

Accuracy achieved: ~97%

##### 6.2 Classification Report

The classification report includes:

➤ Precision

➤ Recall

➤ F1-score

These metrics provide deeper insights into how well the model identifies spam and non-spam messages.

##### 6.3 Confusion Matrix

A confusion matrix was used to visualize:

➤ True Positives (correct spam detection)

➤ True Negatives (correct ham detection)

➤ False Positives

➤ False Negatives

This helped analyze misclassification patterns.

__7. Results and Discussion__

The model demonstrated high accuracy and reliability in detecting spam messages. The Naive Bayes classifier performed exceptionally well due to the probabilistic nature of word occurrence in spam emails. The use of TF-IDF improved the model’s ability to differentiate between meaningful and common words.

Some minor misclassifications occurred due to:

➤ Short or ambiguous messages

➤ Overlapping vocabulary between spam and ham messages

➤ Overall, the results indicate that machine learning is highly effective for spam detection tasks.

__8. Applications__

The developed model can be applied in:

➤ Email filtering systems

➤ SMS spam detection

➤ Customer support automation

➤ Social media content moderation

__9. Limitations__

➤ The model relies on labeled data and may struggle with new spam patterns.

➤ Performance may degrade if language or vocabulary changes significantly.

➤ The dataset contains SMS messages, which may differ slightly from real-world email data.

__10. Conclusion__

This project successfully demonstrates the implementation of a machine learning predictive model using scikit-learn to classify spam emails. By applying TF-IDF feature extraction and a Naive Bayes classifier, the model achieved high accuracy and reliable performance. The project highlights the importance of machine learning techniques in solving real-world text classification problems
