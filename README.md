# Credit_risk_assessment

This project leverages machine learning to assess the credit risk of loan applicants based on various financial and demographic factors. The project includes a trained model, an interactive Streamlit application for real-time predictions, and explainability features using SHAP.

## Features

- **Model Training**: A Gradient Boosting Classifier trained on preprocessed financial data.
- **Interactive Frontend**: A Streamlit-based user interface to input applicant details and receive credit risk predictions.
- **Explainability**: Integration with SHAP to provide insights into model predictions.
- **User-Friendly Interface**: Intuitive input widgets and visual feedback.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/jaydugad/Credit_risk_assessment.git
   cd Credit_Risk_Assessment
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Place the pre-trained model and scaler files (`credit_risk_model.pkl`, `scaler.pkl`) in the project directory.

4. Run the Streamlit app:
   ```bash
   streamlit run app.py
   ```

## How to Use

1. Open the Streamlit app in your browser (the URL will be displayed in the terminal).

2. Enter the applicant's details in the sidebar:
   - Age
   - Annual Income
   - Employment Length
   - Loan Amount
   - Loan Intent
   - Loan Grade
   - Interest Rate
   - Loan Percent of Income
   - Credit History Length
   - Home Ownership
   - Credit Bureau Default Flag

3. Click **Predict Credit Risk** to see the risk score and prediction.

4. (Optional) Click **Explain Prediction** to view SHAP explanations.

## Project Structure

```
.
├── app.py                  # Streamlit application
├── credit_risk_model.pkl   # Trained model file
├── scaler.pkl              # Scaler for preprocessing numerical inputs
├── requirements.txt        # List of dependencies
├── README.md               # Project documentation
```

## Requirements

- Python 3.7+
- Streamlit
- Scikit-learn
- SHAP
- Matplotlib
- Pandas
- Numpy

## Dataset
The dataset used for training the model includes features such as:
- Applicant's age, income, employment length, and home ownership status.
- Loan-related information like amount, purpose, grade, and interest rate.
- Credit history and default status.

## Model

- **Algorithm**: Gradient Boosting Classifier
- **Metrics**: Evaluated using ROC-AUC and classification accuracy.
- **Feature Importance**: Visualised using SHAP values.

## SHAP Integration
The app includes SHAP-based explanations for predictions. Users can view the impact of each feature on the credit risk assessment.

## Contribution
Contributions are welcome! Please create a pull request or open an issue to discuss potential improvements.

## License
This project is licensed under the MIT License. See the LICENSE file for details.

## Acknowledgements
- [Streamlit](https://streamlit.io/)
- [SHAP](https://shap.readthedocs.io/en/latest/)
- [Scikit-learn](https://scikit-learn.org/)

---
For questions or feedback, please contact [www.jaydugad.com].

