# Enhancing Prostate Cancer Prediction with Explainable AI (XAI)

This repository contains the code for a project focused on enhancing prostate cancer prediction using Explainable AI (XAI). The project employs an interpretable Random Forest model and utilizes SHAP (Shapley Additive Explanations) and LIME (Local Interpretable Model-Agnostic Explanations) to provide transparent and actionable insights for clinical decision-making.

## Table of Contents

- [Project Overview](#project-overview)
- [Installation](#installation)
- [Usage](#usage)
- [Results and Discussion](#results-and-discussion)
- [Contributing](#contributing)
- [License](#license)

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

2. Create and activate a virtual environment (optional but recommended):
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate
    ```

3. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. **Train the Model**: 
   Run the `train_model.py` script to train the Random Forest classifier using the prostate cancer dataset. This will also generate SHAP and LIME visualizations.

    ```bash
    python train_model.py
    ```

2. **Model Inference**: 
   Once the model is trained, you can use it to make predictions on new data by running:
   
    ```bash
    python predict.py --input_data path_to_input_data.csv
    ```

3. **View Interpretability Plots**: 
   SHAP and LIME plots will be saved as PNG files, which visualize feature importance and model explanations.

4. **Saving and Loading the Model**: 
   The trained model is saved to a file using `joblib`. You can load it back with:
   
    ```python
    import joblib
    model = joblib.load('best_model.joblib')
    ```

## Results and Discussion

The trained Random Forest model achieved a high accuracy rate for predicting prostate cancer. SHAP and LIME were used to interpret the model, showing the most important features such as `PSAD` (Prostate-Specific Antigen Density) and `Age`. These insights provide transparency to the model's decision-making process, ensuring clinicians can trust the AI's predictions.

## Contributing

Contributions are welcome! If you have suggestions or want to contribute, feel free to fork this repository and open a pull request.


