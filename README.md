# Face Recognition System

A face recognition system built using **Python, OpenCV, and Deep Learning**. The project detects faces from images or a camera feed and uses a trained deep learning model to recognize the person.

## 📌 Project Overview

This project was developed as an **AI/ML project** to understand the complete workflow of a face recognition system — from collecting face images and preprocessing the data to training a deep learning model and deploying it for recognition.

The system uses **OpenCV** for face detection and a trained neural network model for recognizing faces.

## 🎯 Objectives

* Detect human faces using OpenCV.
* Collect and prepare face images for training.
* Preprocess and clean the collected face data.
* Train a deep learning model for face recognition.
* Save the trained model for later use.
* Recognize faces using the trained model.
* Create a simple deployment/inference program for real-time recognition.

## 🧠 How the System Works

The general workflow of the project is:

```text
Face / Camera Input
        ↓
Face Detection
        ↓
Face Cropping
        ↓
Image Preprocessing
        ↓
Trained Deep Learning Model
        ↓
Face Prediction
        ↓
Recognized Person
```

### 1. Face Detection

The project uses the **Haar Cascade Classifier** provided by OpenCV to detect faces.

The classifier used in this project is:

```text
haarcascade_frontalface_default.xml
```

### 2. Data Collection

Face images are collected using:

```text
collect_data.py
```

The collected images are used to create the dataset required for training the recognition model.

### 3. Data Preparation

The collected data is processed and prepared before being given to the model.

The project contains:

```text
consolidated.py
```

for working with and preparing the collected data.

### 4. Model Training

The main training process is contained in:

```text
face_detection (1).ipynb
```

The notebook contains the experimentation and training process used to develop the face recognition model.

### 5. Trained Model

The trained model is saved as:

```text
finalmodel.h5
```

The model is stored using **Git LFS** because of its large file size.

### 6. Deployment

The trained model can be used for recognition through:

```text
deploy (1).py
```

This allows the trained model to be used after training without retraining the entire model.

## 🛠️ Technologies Used

| Technology         | Purpose                               |
| ------------------ | ------------------------------------- |
| Python             | Main programming language             |
| OpenCV             | Face detection and image processing   |
| TensorFlow / Keras | Deep learning model                   |
| NumPy              | Numerical and array operations        |
| Matplotlib         | Visualization                         |
| Jupyter Notebook   | Model development and experimentation |
| Git                | Version control                       |
| Git LFS            | Large model file management           |

## 📂 Project Structure

```text
Face-Recognition/
│
├── collect_data.py
├── consolidated.py
├── deploy (1).py
├── face_detection (1).ipynb
├── finalmodel.h5
├── haarcascade_frontalface_default (2).xml
├── requirements.txt
├── .gitignore
└── .gitattributes
```

### File Description

**`collect_data.py`**
Collects face images that can be used for creating the training dataset.

**`consolidated.py`**
Used for processing/consolidating the collected face data.

**`face_detection (1).ipynb`**
Jupyter Notebook containing the model development, preprocessing, training, and experimentation.

**`deploy (1).py`**
Uses the trained model for face recognition/inference.

**`finalmodel.h5`**
The trained deep learning model.

**`haarcascade_frontalface_default (2).xml`**
OpenCV Haar Cascade classifier used for detecting frontal faces.

**`requirements.txt`**
Contains the Python dependencies required for the project.

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/Jishnu005/Face-Recognition.git
```

```bash
cd Face-Recognition
```

### 2. Install the required packages

It is recommended to create a virtual environment first.

```bash
python -m venv venv
```

Activate it on Windows:

```bash
venv\Scripts\activate
```

Then install the dependencies:

```bash
pip install -r requirements.txt
```

## ▶️ Running the Project

After installing the dependencies, the trained model can be used through the deployment script.

```bash
python "deploy (1).py"
```

The training and experimentation notebook can be opened using Jupyter:

```bash
jupyter notebook
```

Then open:

```text
face_detection (1).ipynb
```

## 📊 Model Performance

The model was trained using the face dataset collected for this project.

**Model performance:**
Add your final validation/test accuracy here after confirming the value from your notebook.

For example:

```text
Training Accuracy: XX%
Validation Accuracy: XX%
```

> The accuracy values should be taken directly from the final training results rather than estimated.

## 🖼️ Results

The system is designed to:

* Detect faces from the input.
* Extract the detected face region.
* Process the face image.
* Pass the processed image to the trained model.
* Predict the corresponding person/class.

You can add screenshots of your actual output here.

Example:

```text
results/
├── detection_result.png
└── recognition_result.png
```

## 🔐 Dataset & Privacy

The original face images used for training are **not included in this public repository**.

This is intentional because face images are biometric data and should not be unnecessarily exposed publicly.

The repository contains the code and trained model required to demonstrate the project without publishing the complete collected dataset.

## 🚀 Future Improvements

Possible improvements for the project include:

* Improve recognition accuracy with a larger and more diverse dataset.
* Add more training samples for each person.
* Improve preprocessing and data augmentation.
* Experiment with modern face recognition architectures.
* Add confidence scores to predictions.
* Improve real-time recognition performance.
* Create a graphical user interface.
* Deploy the model as a web application.
* Add support for recognizing multiple faces simultaneously.
* Improve robustness under different lighting conditions and face angles.

## 📚 What I Learned

Through this project, I gained practical experience with:

* Computer vision using OpenCV.
* Face detection using Haar Cascade.
* Image preprocessing.
* Dataset collection and preparation.
* Deep learning model training.
* Model evaluation.
* Saving and loading trained models.
* Using trained models for inference.
* Structuring an AI/ML project.
* Using Git and GitHub for version control.
* Using Git LFS for managing large machine learning model files.

## 👨‍💻 Author

**Jishnu Mangaraj**

BCA Student | AI/ML Enthusiast

## ⭐ Acknowledgements

This project was developed as a learning project to gain practical experience in **Computer Vision, Deep Learning, and Face Recognition**.
