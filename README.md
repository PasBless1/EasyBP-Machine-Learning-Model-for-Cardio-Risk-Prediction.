# EasyBP: AI-Powered:Cardio-Risk-Prediction and Blood Pressure Monitoring-Model/App

**Project Overview**

EasyBP is a digital health solution designed to transform hypertension management using artificial intelligence and advanced data analytics. By leveraging real-time data streams from wearables, home blood pressure monitors, and electronic health records, EasyBP enables continuous monitoring, risk prediction, and early intervention for cardiovascular disease. The platform integrates a robust ML pipeline and mobile app interface to deliver personalized, actionable insights for both patients and clinicians.

**Motivation**

Hypertension remains a leading risk factor for cardiovascular morbidity and mortality worldwide. Traditional management is hampered by infrequent measurements and delayed therapeutic responses. EasyBP addresses this gap with continuous data collection and predictive analytics, supporting proactive, personalized clinical care and improving patient adherence to treatment routines.

**Data Source**

Dataset: Framingham Heart Study (Kaggle)

Records: 4,240 patients

Features: Age, gender, smoking status, systolic/diastolic BP, BMI, heart rate, cholesterol, glucose, diabetes, medication status, and a binary label for 10-year CHD risk.

Careful preprocessing ensured data quality and ethical compliance, with missing values addressed via imputation and outliers managed to preserve clinical reliability.

**Methodology**

**Data Architecture and Preprocessing**

Integrated pipeline for loading, exploring, cleaning, and transforming patient records.

Addressed missing values and class imbalance (ratio of ~31% positive cases) using SMOTE oversampling and RandomUnderSampler.

Standardized numerical features to ensure comparability and robust modeling.

Retained and engineered features based on clinical relevance and predictive utility.

**Machine Learning Development:**

Designed a complete data pipeline, including advanced cleaning (imputation, outlier treatment with Winsorizing, and class balancing via SMOTE/undersampling), feature engineering, and multi-step scaling/transformation.

Trained and compared four classification algorithms—Random Forest, Logistic Regression, KNN, and XGBoost—to identify the strongest performer.

Selected Random Forest as the final model, achieving an accuracy of 89.7% with minimal false positives and negatives, meeting stringent performance criteria.

Conducted extensive cross-validation and hyperparameter optimization to maximize model generalizability and clinical reliability.

Integrated explainable AI components (feature importance, SHAP/LIME explanations) for model transparency.

<img width="1775" height="1357" alt="image" src="https://github.com/user-attachments/assets/f58b8f97-c211-4891-be3a-b445ed94f057" />

**Model Selection**

A comparative approach evaluated four classifiers:

Random Forest: Selected for its strong balance of sensitivity and specificity, interpretable feature importances, and robustness to noise.

Logistic Regression: Provided a transparent baseline for clinical interpretability.

XGBoost: Leveraged for state-of-the-art structured data performance.

K-Nearest Neighbors (KNN): Intuitive similarity-based prediction.

Random Forest demonstrated the best trade-off between false negatives and overall accuracy, which is crucial for reliable hypertension screening.

**Evaluation**

Metrics: Accuracy, recall, precision, F1-score, and confusion matrix.

Performance:

Accuracy: 89.74%

Recall: 90.75%

Precision: 89.25%

F1-score: 90.00%

Only 21 false negatives out of 1,170 positive cases
These results exceed clinical standards and minimize missed diagnoses in real-world scenarios.

**Deployment**

Model Serialization: Trained Random Forest saved as bpmodel.pkl using joblib.

API Integration: Developed a scalable RESTful API with FastAPI for real-time prediction and mobile deployment.

Voice-Based Input: Integrated speech-to-text for seamless, accessible health data entry.

Mobile Feedback: Real-time risk estimates and personalized interventions delivered to users via app notifications and recommendations.

**Discussion**

**Strengths**
Enables continuous remote monitoring, early risk detection, and proactive care.
Supports both patient self-management and clinician decision-making.
Reduces clinical workload by automating analysis and alerts.
Adaptable and scalable for broader deployment in digital health.

**Limitations**
Data integration and quality remain challenges for universal adoption.
Requires robust technology infrastructure and user digital literacy.
Privacy, security, and regulatory considerations must be addressed in every deployment context.

**Opportunities and Threats**
Potential to expand digital hypertension care to resource-limited settings.
Growing acceptance of digital health creates momentum for adoption.
Equitable access, user resistance, and cybersecurity risks must be proactively managed.

**Conclusion**
EasyBP demonstrates that scalable digital health solutions can achieve high clinical utility with real-world datasets by leveraging robust machine learning, practical deployment, and user-centered design. This project is poised for future growth in proactive cardiovascular risk management, digital health research, and real-life clinical applications, addressing major challenges in precision and accessibility.

**API & App Integration:**
Led API development to seamlessly connect the trained model with the EasyBp app, ensuring that user data is processed and risk scores are delivered instantly and securely.
Designed user-friendly interfaces for inputting health metrics and receiving actionable feedback.

**Technical Highlights**

**Advanced data preprocessing:** 
Handling missing values, outliers, and class imbalance for robust model input.
Multi-algorithm model benchmarking and interpretability.

**Explainable AI:**
Enabled global and instance-level model explanation through feature importance analysis and SHAP/LIME for transparent predictions.
Automated end-to-end pipeline for real-time prediction and model deployment.

**Achievements**
Delivered a clinically relevant digital health tool that bridges ML research and practical patient-centered care.
Promoted data-driven personalization and preventative health strategies.
Strengthened collaborative development, API design, and full-stack ML deployment skills.

This project is a testament to the power of combining rigorous machine learning, explainable AI, and practical software engineering to tackle real-world healthcare challenges.
