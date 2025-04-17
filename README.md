# plant_disease_detection
Plant Leaf Disease Detection
Overview
This project uses Convolutional Neural Networks (CNN) to detect diseases in plant leaves. It's implemented as a web application using Flask, allowing users to upload images of plant leaves and receive real-time disease detection results. The system can identify healthy leaves as well as those affected by powdery mildew and rust diseases.
Features

Deep Learning Model: CNN-based model for accurate leaf disease detection
Web Interface: User-friendly interface built with Flask
Real-time Analysis: Instant disease detection from uploaded images
Multi-class Classification: Detects multiple disease categories (Healthy, Powdery Mildew, Rust)
High Accuracy: Pre-trained model with optimized performance

Technologies Used

Python: Core programming language
TensorFlow/Keras: Deep learning framework for CNN implementation
Flask: Web framework for the application
OpenCV: Image processing library
PIL (Python Imaging Library): Additional image processing functionality
NumPy: Numerical computing
HTML/CSS/JavaScript: Frontend development

Installation
Prerequisites

Python 3.6+
pip package manager

Setup

Clone the repository

bashgit clone https://github.com/yourusername/plant-disease-detection.git
cd plant-disease-detection

Create a virtual environment (optional but recommended)

bashpython -m venv venv
source venv/bin/activate  # On Windows, use: venv\Scripts\activate

Install dependencies

bashpip install tensorflow numpy pillow opencv-python flask werkzeug
Usage
Running the Application

Ensure the model file 'model.h5' is in the root directory
Start the Flask server

bashpython app.py

Open your web browser and navigate to http://127.0.0.1:5000/

Making Predictions

Use the web interface to upload an image of a plant leaf
Click the submit button to process the image
View the prediction result (Healthy, Powdery Mildew, or Rust)

Project Structure
plant-disease-detection/
├── app.py                  # Flask application (main code)
├── model.h5                # Trained CNN model
├── static/                 # Static files (CSS, JS, images)
├── templates/              # HTML templates
│   └── index.html          # Main page template
├── uploads/                # Directory for uploaded images
└── README.md               # This file
Model Information

Architecture: Convolutional Neural Network (CNN)
Input Size: 225x225 pixel images
Classes: 3 (Healthy, Powdery Mildew, Rust)
Framework: TensorFlow/Keras

How It Works

User uploads an image through the web interface
The image is preprocessed (resized to 225x225 pixels and normalized)
The preprocessed image is fed to the pre-trained CNN model
The model predicts the probability of each disease class
The class with the highest probability is returned as the result

Future Improvements

Add support for more plant types and diseases
Implement detailed disease information and treatment recommendations
Add a confidence score with the prediction
Improve the user interface with result visualization
Develop a mobile application version


Plant disease datasets used for training the model
TensorFlow and Keras documentation
Flask web framework

Contact
For questions or support, please contact sanjay.cse.ds@example.com
