# Rice Leaf Disease Classification using Deep Learning

## Project Overview
This project focuses on classifying rice leaf diseases using deep learning techniques.
The objective is to build an image classification model that can identify different
rice leaf conditions from images.

The project was completed strictly using the dataset and guidelines provided by
the institute as part of the academic submission.

---

## Dataset Description
The dataset consists of rice leaf images categorized into three classes:
- **Brown Spot**
- **Leaf Smut**
- **Bacterial Leaf Blight**

The dataset is limited in size and was provided by the institute.
Additional images were used only for testing and understanding model behavior.

---

## Project Structure

Rice-Leaf-Disease-Classification/
│
├── data/
│ ├── raw/ # Original training images
│ └── test/ # Test images for prediction
│
├── models/
│
│└── rice_leaf_classifier.keras
│
├── notebooks/
│ └── final_submission.ipynb
│
├── README.md
├── requirements.txt


---
## Methodology
1. **Data Loading & Preprocessing**
   - Images were resized to a fixed dimension
   - Pixel values were normalized
   - Data augmentation was applied to reduce overfitting

2. **Model Architecture**
   - Transfer learning using **MobileNetV2**
   - Pretrained convolutional layers were frozen
   - Custom dense layers were added for classification

3. **Model Training**
   - Categorical Crossentropy loss function
   - Adam optimizer
   - Early stopping and model checkpointing used

4. **Evaluation**
   - Model evaluated using validation accuracy and loss
   - Predictions performed on unseen test images

---

## Results
- The model achieved high validation accuracy during training.
- Due to the small dataset size, some overfitting behavior was observed.
- Performance may vary when tested on external real-world images.

---

## Observations & Limitations
- The dataset size is limited, which impacts generalization
- High validation accuracy does not guarantee real-world robustness
- Further improvement requires larger and more diverse datasets

---

## Conclusion
This project demonstrates the application of transfer learning for image classification
using a small dataset. The results are satisfactory within the constraints of the
provided data and serve as a foundational deep learning implementation.

---

## Tools & Technologies Used
- Python
- TensorFlow / Keras
- NumPy
- Matplotlib
- Jupyter Notebook

---

## Submission Notes
- Model performance is limited by dataset size
- The project follows the instructions provided by the institute
