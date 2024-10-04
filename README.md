# Customer Churn Analysis

## Description
This project is part of an assignment for IS470, designed to evaluate the understanding of data mining, 
particularly classification problems using decision trees. The project explores 
customer churn, which refers to the phenomenon where customers discontinue their relationship 
with a business. The goal is to help businesses predict potential customer churn based on 
given attributes using Python and SQL for analysis.

## Dataset
The dataset used in this project is **CustomerChurnData.csv**, which contains various customer attributes. 
The objective is to use these attributes to predict whether a customer will churn or not.

## Technologies Used
- **Python**: For data analysis and visualization.
- **SQL**: For querying and handling the dataset.
- **Google Colab**: Used to execute and document the entire data mining process.

## Data Mining Process
This project follows the **CRISP-DM** framework:
1. **Understanding the domain**: Analysis of customer churn through literature review.
2. **Data understanding and preprocessing**: Visualizing the data, handling missing values, and identifying key variables.
3. **Decision Tree Classifier**: Developed a decision tree to classify churn (Y/N).
4. **Model Evaluation**: Performance metrics like accuracy, sensitivity (recall), precision, F-measure, and confusion matrix are calculated.
5. **Feature Importance**: Discussed the variables with the highest impact on churn prediction.

## Key Features
- **Data Visualization**: Includes various charts to explore data patterns (limited to 10 charts).
- **Decision Tree**: A classifier model to predict customer churn.
- **Model Performance Metrics**: Evaluated using accuracy, recall, precision, F-measure, and confusion matrix.
- **Feature Analysis**: Identification of important variables contributing to churn prediction.

## Results and Conclusion
The model achieved an overall accuracy of 87%, which indicates it performs quite well.
However, after analyzing deeper, the model's performance in identifiying churners was lacking. While the precision for churners was 80%, 
the recall was only 72%, meaing 28% of the actual churners were not identified by the model! 
This can have serious implications for businesses relying on the model to retain at-risk customers, 
since missed churners could leave without any retention effort.

Strengths of my approach would include:
The model's overall performance, especially identfiying non-churners. (for promotions, etc)
The accuracy and precision for classifying customers as non-churners, 
which show the model can be trusted for a large portion of the customer base.

Weaknesses in my approach would include:
The recall for churners is not as high as desired. The model missed 28% of actual churners, which limits its effectiveness for businesses.
No balancing was used during this project which might have made the model much better.

While the model provides a foundation for predicting customer churn, 
I think businessess should be cautious when relying solely on this classifier. It's current strengths lie with identifying non-churners accurately, 
which is not the intended use of the model. The model was made to capture all at-risk customers, and it fails to do so 28% of the time.

## How to Use
To view the project:
- Open the provided `.html` file to see the analysis and results.
- Ensure you have access to the **CustomerChurnData.csv** dataset if you wish to replicate the analysis.

## Author
Rafael Melkumian

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
