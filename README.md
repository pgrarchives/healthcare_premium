# Health Insurance Cost Predictor

![Health Insurance Cost Predictor UI](https://healthcarepremium.streamlit.app)

## Overview
The Health Insurance Cost Predictor is a web-based application designed to predict health insurance premiums based on a variety of user input factors. The application is built using a public dataset and developed with a combination of Streamlit, Python, and machine learning models. This project focuses on predicting the health insurance cost based on several factors like age, gender, smoking status, region, and more.

The project utilizes two different machine learning models to provide the best prediction results based on the user's age category:
- **Linear Regression** for users **under 25 years of age**.
- **XGBoost** for users **above 25 years of age**.

The models were selected based on accuracy and performance, where Linear Regression performed well for younger individuals while XGBoost provided better accuracy for the older age group.

## Table of Contents
- [Overview](#overview)
- [Application Screenshot](#application-screenshot)
- [Technologies Used](#technologies-used)
- [Project Structure](#project-structure)
- [How to Run](#how-to-run)
- [License](#license)

## Application Screenshot
![App Interface](image.png)

## Technologies Used
- **Python**: Backend programming language used to create the models and application logic.
- **Streamlit**: Python-based framework used to create the web interface for the application.
- **Scikit-Learn**: Utilized for the Linear Regression model and data preprocessing.
- **XGBoost**: Model chosen for users above 25 years for improved accuracy.

## Project Structure
```
HEALTHCARE_PREMIUM/
├── artifacts/
│   ├── model_rest.joblib          # Model for individuals above 25 years
│   ├── model_young.joblib         # Model for individuals under 25 years
│   ├── scaler_rest.joblib         # Scaler for individuals above 25 years
│   ├── scaler_young.joblib        # Scaler for individuals under 25 years
├── LICENSE
├── main.py                 # Main file for running the application
├── prediction_helper.py     # Helper functions for predictions
├── README.md
├── requirements.txt       # Python dependencies for the project
```

## How to Run
1. **Clone the Repository**:
   ```
   git clone https://github.com/yourusername/healthcare_premium.git
   cd healthcare_premium
   ```

2. **Install Dependencies**:
   Ensure you have Python installed, then use pip to install the dependencies.
   ```
   pip install -r requirements.txt
   ```

3. **Run the Application**:
   Launch the Streamlit application with the following command:
   ```
   streamlit run main.py
   ```

4. **Access the Web Application**:
   Open your browser and navigate to `http://localhost:8501` to interact with the application.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Feel free to explore and contribute to the project by creating issues, pull requests, or by reaching out for collaboration.

