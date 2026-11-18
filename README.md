# 🌿 Plant Disease Detection Using Convolutional Neural Networks (CNN)

## 📌 Project Overview
Plant Disease Detection Using CNN is a deep learning-based project that identifies plant diseases by analyzing images of plant leaves. The system uses a Convolutional Neural Network (CNN) to classify leaf images into 15 different categories, covering healthy and diseased conditions of Pepper, Potato, and Tomato plants.
The application provides a user-friendly interface developed using Streamlit, allowing users to upload leaf images and view the predicted disease class along with its confidence score.

## 🎯 Objectives
- Detect plant diseases using leaf images.
- Develop a CNN model for multiclass image classification.
- Classify healthy and diseased leaves into 15 categories.
- Evaluate model performance using standard evaluation metrics.
- Develop an interactive interface for image upload and disease prediction.

## 🗂️ Dataset
- **Dataset:** PlantVillage Dataset
- **Source:** Kaggle
- **Total Images:** 20,638
- **Total Classes:** 15
- **Plant Categories:** Pepper, Potato, and Tomato.

### Dataset Distribution
| Dataset | Images | Percentage |
|---|---:|---:|
| Training | 14,440 | 70% |
| Validation | 3,097 | 15% |
| Testing | 3,101 | 15% |
| **Total** | **20,638** | **100%** |

Dataset Link: https://www.kaggle.com/datasets/emmarex/plantdisease

## 🛠️ Technologies Used
- **Programming Language:** Python
- **Deep Learning Framework:** TensorFlow / Keras
- **Model:** Convolutional Neural Network (CNN)
- **Frontend:** Streamlit
- **Image Processing:** Pillow
- **Numerical Computing:** NumPy
- **Data Visualization:** Matplotlib
- **Evaluation:** Scikit-learn
- **Development Environment:** Google Colab

## 🧠 CNN Architecture
The project uses a Sequential CNN architecture consisting of:
1. Convolutional Layer (32 filters)
2. Max Pooling Layer
3. Convolutional Layer (64 filters)
4. Max Pooling Layer
5. Convolutional Layer (128 filters)
6. Max Pooling Layer
7. Global Average Pooling
8. Dropout Layer (30%)
9. Dense Layer (128 neurons)
10. Output Layer (15 neurons with Softmax activation)

**Model Configuration:**
- Optimizer: Adam
- Learning Rate: 0.001
- Loss Function: Sparse Categorical Cross-Entropy
- Batch Size: 32
- Maximum Epochs: 20
- Trainable Parameters: 111,695

## ⚙️ Image Preprocessing
The following preprocessing operations are performed:
- Image resizing to 128 × 128 pixels.
- RGB colour conversion.
- Pixel normalization from 0–255 to 0–1.
- Batch loading using a batch size of 32.

## 📊 Model Performance
The trained CNN model was evaluated using 3,101 unseen test images.
| Evaluation Metric | Result |
|---|---:|
| Test Accuracy | **93.58%** |
| Test Loss | 0.2084 |
| Correct Predictions | 2,902 |
| Incorrect Predictions | 199 |
| Macro F1-Score | 93.15% |
| Weighted F1-Score | 93.56% |

The model was further evaluated using a confusion matrix, classification report, precision, recall, and F1-score.

## 🖥️ Application Features
- Simple and interactive Streamlit interface.
- Upload plant leaf images.
- Preview uploaded images.
- Automatic image preprocessing.
- CNN-based disease classification.
- Display predicted disease category.
- Display prediction confidence score.
- Error handling for invalid inputs and missing files.

## 🔄 Project Workflow
1. Dataset Collection
2. Dataset Inspection and Organization
3. Image Preprocessing
4. CNN Model Development
5. Model Training and Validation
6. Model Testing and Evaluation
7. Streamlit Interface Development
8. Disease Prediction and Result Display

## 🚀 Installation and Execution
**1. Clone the repository**
```bash
git clone <repository-url>
cd Plant-Disease-Detection
```
**2. Install the required libraries**
```bash
pip install tensorflow streamlit numpy pillow matplotlib scikit-learn
```
**3. Ensure the trained model and class mapping files are available**
- `plant_disease_cnn.keras`
- `class_names.json`
**4. Run the application**
```bash
streamlit run app.py
```
**5. Upload a plant leaf image and view the prediction.**

## 🔮 Future Enhancements
- Extend disease detection to more plant species.
- Improve model accuracy and generalization.
- Integrate disease-specific treatment recommendations.
- Develop a mobile application.
- Explore real-time plant disease detection.

## 👩‍💻 Project Team 
1. **Saniya Nawaz**
2. **Sathya S**
3. **Tanzila Siddiqa**
4. **Tasmiya A**

## 📌 Conclusion
This project demonstrates the application of deep learning and computer vision in agricultural disease identification. By combining CNN-based image classification with an interactive Streamlit application, the system provides an accessible approach to identifying plant diseases from leaf images.
---
⭐ If you find this project useful, consider giving the repository a star!
**Note:** This project is developed for academic and educational purposes. Model predictions should be verified before making real-world agricultural treatment decisions.
