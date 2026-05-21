\# Pneumonia Detection from Chest X-Ray Images Using CNNs and Transfer Learning



\## Project Overview



This project was developed as part of the CMP600 Dissertation module for the BSc (Hons) Computing Top-up programme. The aim of the project is to investigate how deep learning techniques can be applied to detect pneumonia from chest X-ray images.



Three models were implemented and compared:



\- Baseline Convolutional Neural Network (CNN)

\- VGG16 transfer-learning model

\- ResNet50 transfer-learning model



The project was implemented in Google Colab using Python, TensorFlow and Keras.



\## Dataset



The project uses the publicly available Kaggle Chest X-Ray Pneumonia dataset:



https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia



The dataset is not included in this repository due to size and licensing considerations. Users should download it directly from Kaggle.



\## Methodology



The implementation includes:



\- Dataset loading and verification

\- Image resizing to 224 x 224 pixels

\- Normalisation

\- Data augmentation

\- 80/20 training-validation split

\- Class weighting to reduce dataset imbalance

\- Training with EarlyStopping

\- Model checkpoint saving every 10 epochs

\- Evaluation using accuracy, precision, recall, specificity, F1-score and ROC-AUC

\- Grad-CAM explainability for VGG16



\## Final Results



| Model | Accuracy | Precision | Recall/Sensitivity | Specificity | F1-score | ROC-AUC |

|---|---:|---:|---:|---:|---:|---:|

| Baseline CNN | 0.832 | 0.794 | 0.987 | 0.573 | 0.880 | 0.948 |

| VGG16 | 0.888 | 0.857 | 0.985 | 0.726 | 0.916 | 0.967 |

| ResNet50 | 0.782 | 0.813 | 0.846 | 0.675 | 0.829 | 0.851 |



VGG16 achieved the best overall performance and was selected as the strongest model in this study.



\## Explainability



Grad-CAM was applied to the VGG16 model to visualise which areas of the chest X-ray influenced the prediction. The model mainly focused on the central chest and lung regions, supporting model interpretability.



\## Tools and Technologies



\- Python

\- TensorFlow / Keras

\- Google Colab

\- Scikit-learn

\- Matplotlib

\- Seaborn

\- OpenCV

\- Kaggle API



\## Ethical Considerations



This project uses publicly available anonymised secondary data. No primary data collection or human participant involvement was conducted. The model is intended as a research prototype and decision-support artefact, not as a replacement for clinical judgement.



\## Author



Ion Cojocaru  

BSc (Hons) Computing \[Top-up]  

Elizabeth School of London  

CMP600 Dissertation

