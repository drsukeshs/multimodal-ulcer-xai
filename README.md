# multimodal-ulcer-xai
![Slide1](https://github.com/user-attachments/assets/aeef9def-dc79-49e9-afee-fb9e8f865836)

Multimodal deep learning pipeline to classify common wounds in surgical practice, with implementation of SHAP for explainability of models predictions

## Overview

This project demonstrates a multimodal deep learning pipeline for classifying skin ulcers using tabular clinical data and wound images.

Due to the scarcity of clinical ulcer data, some standard evaluation metrics like AUROC and F1-score are not fully representative for this dataset. Instead, the focus is on demonstrating a robust workflow, including:

Expert data cleaning: All images manually verified and curated using clinical knowledge

Synthetic tabular data generation: Populated realistic patient and wound features in a CSV

Multimodal model implementation: Combines tabular + image inputs for predictions

Explainability with SHAP: Provides insights into which tabular features influence predictions

Evaluation with available metrics: Accuracy and confusion matrix to illustrate model behavior

⚠️ Results are for demonstration purposes only and not clinically validated. The emphasis is on pipeline development, data handling, and explainable AI rather than benchmark performance.
## Dataset
Image dataset compiled from multiple sources, processed and stored as .jpeg files.

Clinical data stored in tabular form in .csv format with a combination of numerical values and strings (one hot encoded for use later).

Dataset: CSV :https://www.kaggle.com/datasets/therealsukeshs/uuuuuiii/data
          Images: https://www.kaggle.com/datasets/therealsukeshs/ulcer-dataset-kaggle1
          
## Key Highlights

Manual image curation leveraging medical expertise

Synthetic clinical tabular data for multimodal fusion

Autokeras automated model search for efficient architecture selection

SHAP explainability for tabular features

## Limitations

Small dataset → some classes mildly underrepresented

AUROC and F1-score may be inaccurate due to limited validation samples

Results are demonstrational and not intended for clinical decision-making

## Future Work

Expand dataset with additional clinical images

Implement class balancing and cross-validation

Add advanced image explainability

Fine-tune multimodal architecture for improved predictions
