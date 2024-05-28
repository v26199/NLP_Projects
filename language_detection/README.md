# Language Detection Model

## Dataset Introduction
The dataset consists of text data for 17 different languages, including English, Malayalam, Hindi, Tamil, Kannada, French, Spanish, Portuguese, Italian, Russian, Swedish, Dutch, Arabic, Turkish, German, Danish, and Greek.

## Steps Involved

1. **Data Labeling**: The dataset is labeled to assign target labels to the data.

2. **Text Data Preprocessing**: 
   - Text data is preprocessed to remove noise, such as special characters, punctuation, and stopwords.
   - Text is tokenized and converted to lowercase for uniformity.
   
3. **Train-Test Split**: The preprocessed data is split into training and testing sets for model evaluation.

4. **Vectorization**: Preprocessed text data is transformed into numerical vectors using TF-IDF vectorization.

5. **Model Building and Training**: Different models, including Logistic Regression, K-Nearest Neighbors, Random Forest, Naive Bayes, and Artificial Neural Network (ANN), are created and trained.

6. **Model Evaluation**: The trained models are evaluated on both the training and testing data, and results such as accuracy, precision, recall, and F1 score are printed. Additionally, the results are saved into a CSV file.

7. **Comparison of Results**: The saved CSV file is loaded to compare the performance of each model.

## Results and Conclusion

### Logistic Regression:
- **Train Accuracy**: 97.09%
- **Test Accuracy**: 95.38%
- **Key Insights**: Achieved high accuracy across most classes.

### K-Nearest Neighbors:
- **Train Accuracy**: 51.22%
- **Test Accuracy**: 37.08%
- **Key Insights**: Significantly lower performance compared to other models.

### Random Forest:
- **Train Accuracy**: 97.50%
- **Test Accuracy**: 94.11%
- **Key Insights**: High accuracy overall, struggled slightly in classifying certain classes.

### Naive Bayes:
- **Train Accuracy**: 96.41%
- **Test Accuracy**: 96.01%
- **Key Insights**: Balanced performance across all classes.

### Artificial Neural Network (ANN):
- **Test Loss**: 0.135
- **Test Accuracy**: 95.96%
- **Precision**: 96.76%
- **Recall**: 95.96%
- **F1 Score**: 96.14%
- **Key Insights**: Achieved high accuracy and balanced performance across all classes.

Overall, Naive Bayes and the Artificial Neural Network outperformed the other models in terms of both accuracy and F1 score. Logistic Regression and Random Forest also showed commendable performance. However, K-Nearest Neighbors demonstrated the weakest performance, indicating that its simplistic approach might not be suitable for this classification task. This analysis provides valuable insights for future model selection and optimization.
