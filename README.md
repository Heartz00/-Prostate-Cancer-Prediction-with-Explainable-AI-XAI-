# Enhancing Prostate Cancer Prediction with Explainable AI (XAI)

This repository contains the code for a project focused on enhancing prostate cancer prediction using Explainable AI (XAI). The project employs an interpretable Random Forest model and utilizes SHAP (Shapley Additive Explanations) and LIME (Local Interpretable Model-Agnostic Explanations) to provide transparent and actionable insights for clinical decision-making.


## Project Overview

Prostate cancer is one of the most common types of cancer affecting men worldwide. Early detection is crucial, and AI models have shown promising results in predicting the likelihood of prostate cancer. However, for AI systems to be adopted in clinical settings, their predictions must be interpretable.

This project focuses on training a Random Forest classifier on clinical data for prostate cancer prediction and then applying SHAP and LIME to interpret the model's predictions.

Key features of the project include:
- **Random Forest Model**: Trained on prostate cancer clinical data.
- **SHAP**: Provides global interpretability by highlighting the most important features influencing model predictions.
- **LIME**: Offers local interpretability, explaining individual predictions for specific patients.
- **Model Saving and Loading**: The trained model is saved using `joblib` for easy deployment.

## Installation

To run this project locally, follow these steps:

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/prostate-cancer-prediction-xai.git
    cd prostate-cancer-prediction-xai
    ```

2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```


## Results and Discussion

The trained Random Forest model achieved a high accuracy rate for predicting prostate cancer. SHAP and LIME were used to interpret the model, showing the most important features such as `PSAD` (Prostate-Specific Antigen Density) and `Age`. These insights provide transparency to the model's decision-making process, ensuring clinicians can trust the AI's predictions.

## Contributing

Contributions are welcome! If you have suggestions or want to contribute, feel free to fork this repository and open a pull request.


