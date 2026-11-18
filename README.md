# 🍎 Fruit Recognition Using OpenCV and Machine Learning

## 📌 Project Overview

Fruit Recognition Using OpenCV is a machine learning-based image classification project developed to identify and classify different types of fruits from digital images.

The project uses **OpenCV (Open Source Computer Vision Library)** for image processing and feature extraction, followed by machine learning algorithms to recognize fruit categories.

The system classifies images into four different fruit categories: Apple, Banana, Mango, and Orange.

The main objective of this project is to understand how image preprocessing techniques and traditional machine learning algorithms can be combined to develop an image classification system.

## 🎯 Project Objectives

- Develop a fruit image classification system using Python and OpenCV.
- Understand image processing and feature extraction techniques.
- Convert images into numerical representations suitable for machine learning.
- Implement and compare K-Nearest Neighbors (KNN) and Decision Tree algorithms.
- Evaluate model performance using accuracy scores.
- Predict fruit categories for new input images.

## 📂 Dataset Description

The dataset contains images belonging to four fruit categories:

| Fruit Category | Label |
|---|---|
| Apple | Apple |
| Banana | Banana |
| Mango | Mango |
| Orange | Orange |

The dataset contains 120 images in the notebook's demonstrated run.

Each image is processed and converted into a numerical representation before being passed to the machine learning models.

## 🛠️ Technologies and Libraries Used

- **Python:** Main programming language.
- **OpenCV:** Image reading, grayscale conversion and image resizing.
- **NumPy:** Numerical operations and array manipulation.
- **Pandas:** Dataset creation and data manipulation.
- **Scikit-learn:** Machine learning model development and evaluation.
- **Matplotlib:** Image visualization.
- **Jupyter Notebook:** Development and execution environment.

## ⚙️ Project Workflow

### 1. Library Importing

Imported the required Python libraries, including OpenCV, Pandas, NumPy, OS and ZIP file handling libraries.

### 2. Dataset Extraction

Extracted the fruit image dataset from a ZIP file and organized images into their respective fruit category folders.

### 3. Image Loading Using OpenCV

Used `cv2.imread()` to read the images from the dataset.

### 4. Image Preprocessing

Applied the following preprocessing techniques:

- Converted images into grayscale using OpenCV.
- Resized all images into 28 × 28 pixels.
- Flattened the resized images into one-dimensional arrays.

### 5. Feature Extraction

Each image was converted into a numerical feature vector.

Since every image has a dimension of 28 × 28 pixels:

**28 × 28 = 784 features**

Therefore, each image is represented using 784 pixel intensity values.

### 6. DataFrame Creation

Used Pandas DataFrames to organize the extracted image features and their corresponding fruit labels.

- Created a feature DataFrame.
- Created a label DataFrame.
- Combined both DataFrames.
- Separated independent variables (X) and dependent variable (y).

### 7. Train-Test Split

Used Scikit-learn's `train_test_split()` to divide the dataset into training and testing sets.

- Training data: 80%
- Testing data: 20%
- Random state: 42
- Stratified sampling: Enabled

### 8. Model Building

Implemented two machine learning classification algorithms.

**K-Nearest Neighbors (KNN)**

KNN classifies fruit images by identifying the nearest data points based on feature similarity and assigning the most common class among the neighbors.

**Decision Tree Classifier**

The Decision Tree algorithm learns decision rules from the training data and uses those rules to classify new fruit images.

### 9. Model Evaluation

Evaluated both classification algorithms using the accuracy score metric to compare their performance on the test dataset.

### 10. Image Prediction

Developed a custom prediction function that:

- Reads a new fruit image.
- Converts it into grayscale.
- Resizes it to 28 × 28 pixels.
- Flattens the image into 784 features.
- Predicts the fruit category using the trained model.

## 📊 Model Performance

The following accuracy scores were recorded in the demonstrated notebook execution.

| Algorithm | Accuracy |
|---|---:|
| K-Nearest Neighbors (KNN) | 79.17% |
| Decision Tree Classifier | 100% |

**Observation:**

The Decision Tree classifier achieved higher test accuracy than KNN in this particular experiment.

However, the evaluation was performed on a relatively small dataset containing 120 images, with only 24 images in the test set. Therefore, further testing with a larger and more diverse dataset is necessary before concluding that the Decision Tree model generalizes better.

## 🔍 Prediction and Testing

The trained model can predict fruit categories from new images.

Supported fruit categories:

- Apple
- Banana
- Mango
- Orange

The prediction function accepts an image path and returns the predicted fruit category.

## 📁 Project Structure

```text
Fruit-Recognition-using-OpenCV/
│
├── Fruit_Recognition_OpenCV.ipynb
│
├── README.md
│
├── requirements.txt
│
└── Screenshots/
    └── model_results.png
```

## 🚀 How to Run the Project

**Step 1: Clone the repository**

```bash
git clone https://github.com/SaiLeela88/Fruit-Recognition-using-OpenCV.git
```

**Step 2: Navigate to the project directory**

```bash
cd Fruit-Recognition-using-OpenCV
```

**Step 3: Install the required libraries**

```bash
pip install -r requirements.txt
```

**Step 4: Download and extract the fruit image dataset.**

**Step 5: Update the dataset path in the Jupyter Notebook according to your system.**

**Step 6: Launch Jupyter Notebook**

```bash
jupyter notebook
```

**Step 7: Open the notebook and execute all cells sequentially.**

## 💡 Key Learnings

Through this project, I gained practical experience in:

- Image processing using OpenCV.
- Image resizing and grayscale conversion.
- Feature extraction from images.
- Converting images into numerical arrays.
- Data manipulation using Pandas and NumPy.
- Implementing KNN and Decision Tree classifiers.
- Training and testing machine learning models.
- Evaluating classification performance.
- Building image prediction functions.

## 🔮 Future Enhancements

- Increase the size and diversity of the fruit image dataset.
- Apply image augmentation techniques.
- Experiment with different KNN parameters.
- Improve model generalization through cross-validation.
- Explore advanced machine learning and deep learning approaches such as CNN.
- Develop a user-friendly interface for real-time fruit recognition.

## 👩‍💻 Author

**Sai Leela**

GitHub: https://github.com/SaiLeela88

LinkedIn: https://www.linkedin.com/in/sai-leela-958497371/

---

⭐ If you find this project useful, feel free to explore the repository and share your feedback.

**Project Domain:** Machine Learning | Computer Vision | Image Classification
