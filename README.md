# Loan Default Prediction and Risk Profiling

This is a minor project that builds a hybrid AI model to predict loan default probability and profile borrower risk.

## 🔑 Project Goal

The system combines unsupervised deep learning (Autoencoders) with supervised machine learning (Logistic Regression) to identify high-risk applicants, detect anomalies, and provide interpretable risk profiles.

# 📊 Key Results

# 1. Anomaly Detection (Autoencoder)
The autoencoder was trained on "normal" (non-defaulting) applicants. As a result, it got very good at spotting "weird" or "anomalous" applicants (defaulters), who have a much higher reconstruction error. This proves the core concept of the project.

[Reconstruction Error Plot]
<img width="859" height="552" alt="Reconstruction error" src="https://github.com/user-attachments/assets/0f08b68a-cd34-455c-848f-77efb9453874" />

# 2. Explainable AI (SHAP)
The final hybrid model relies heavily on our new "weirdness score" (`RECON_ERROR`). The SHAP plot shows that `RECON_ERROR` is the **#1 most important feature** for predicting a default. A high error strongly pushes the model to predict "default."

[SHAP Summary Plot]<img width="793" height="940" alt="SHAP" src="https://github.com/user-attachments/assets/1ef95c07-adc3-4c04-96ae-4c21f796739d" />
