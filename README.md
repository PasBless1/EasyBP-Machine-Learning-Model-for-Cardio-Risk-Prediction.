# Machine-Learning-Model-for-Cardio-Risk-Prediction-EasyBP
EasyBp is a collaborative digital health project developed during my Master’s in Digital Health program. The application empowers users and clinicians to track hypertension and receive individualized cardiovascular risk assessments using robust machine learning techniques.

**Project Scope**
Dataset: Leveraged the comprehensive, real-world Framingham Heart Study dataset for developing and validating the predictive model.

**Machine Learning Development:**

Designed a complete data pipeline, including advanced cleaning (imputation, outlier treatment with Winsorizing, and class balancing via SMOTE/undersampling), feature engineering, and multi-step scaling/transformation.

Trained and compared four classification algorithms—Random Forest, Logistic Regression, KNN, and XGBoost—to identify the strongest performer.

Selected Random Forest as the final model, achieving an accuracy of 89.7% with minimal false positives and negatives, meeting stringent performance criteria.

Conducted extensive cross-validation and hyperparameter optimization to maximize model generalizability and clinical reliability.

Integrated explainable AI components (feature importance, SHAP/LIME explanations) for model transparency.

**API & App Integration:**

Led API development to seamlessly connect the trained model with the EasyBp app, ensuring that user data is processed and risk scores are delivered instantly and securely.

Designed user-friendly interfaces for inputting health metrics and receiving actionable feedback.

**Technical Highlights**
**Advanced data preprocessing:** Handling missing values, outliers, and class imbalance for robust model input.

Multi-algorithm model benchmarking and interpretability.

**Explainable AI:** Enabled global and instance-level model explanation through feature importance analysis and SHAP/LIME for transparent predictions.

Automated end-to-end pipeline for real-time prediction and model deployment.

**Achievements**
Delivered a clinically relevant digital health tool that bridges ML research and practical patient-centered care.

Promoted data-driven personalization and preventative health strategies.

Strengthened collaborative development, API design, and full-stack ML deployment skills.

This project is a testament to the power of combining rigorous machine learning, explainable AI, and practical software engineering to tackle real-world healthcare challenges.
