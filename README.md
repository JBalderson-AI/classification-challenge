# Spam Email Classification Challenge
Module 13: Spam Classification

## Overview
This project involves building a supervised machine learning model to classify emails as either spam or not spam. The dataset contains email features and a binary classification label, where `0` represents legitimate emails and `1` represents spam.

## Models Used
Two classification models were implemented and evaluated for performance:
1. **Logistic Regression**
2. **Random Forest Classifier**

## Project Workflow
The following steps were taken to complete the challenge:

1. **Data Loading & Preprocessing**  
   - The dataset was read into a Pandas DataFrame.
   - The `spam` column was used as the target variable (`y`), and the remaining columns were used as features (`X`).
   - The dataset was split into training and testing sets (80% training, 20% testing).
   
2. **Feature Scaling**  
   - The features were standardized using `StandardScaler` to improve model performance.
   
3. **Model Training & Prediction**  
   - A **Logistic Regression model** was trained using the scaled data and used to make predictions.
   - A **Random Forest model** was also trained on the same data and used to make predictions.
   
4. **Model Evaluation**  
   - The accuracy of both models was calculated and compared.
   - Random Forest performed better due to its ability to capture complex relationships and reduce overfitting through ensemble learning.

## Results
| Model                 | Accuracy  |
|----------------------|-----------|
| Logistic Regression  | *93%*    |
| Random Forest       | *96%*    |

## Key Takeaways
- **Random Forest performed better** than Logistic Regression because it leverages multiple decision trees, reducing overfitting and improving predictive power for non-linear relationships.
- **Feature scaling** was crucial for Logistic Regression but less impactful for Random Forest, which is less sensitive to feature magnitudes.


## Author
Jill Balderson

## License
This project is licensed under the MIT License.

