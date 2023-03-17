# Sign_language_detector

This Python project utilizes computer vision and machine learning to detect and recognize American Sign Language (ASL) alphabets A, B, and C in real-time through the webcam.

## Requirements
To run this project, you need:

Python 3.6 or later  
OpenCV 4.2.0 or later  
Numpy 1.19.3 or later


## Installation
1. Clone this repository to your local machine using the following command:  
`!git clone https://github.com/Ahmar1997/document-scanner-using-OpenCV.git`

2. Install the required Python packages by running the following command:  
`pip install opencv-python`  
`pip install numpy`  

3. Data Collection
The dataCollection.py script allows you to collect training data using your webcam.

To collect data for a specific alphabet (e.g. A) change the variable `folder` to A, B or C to collect respective images and run the following command: 
`python collect_data.py`  

You can collect data for multiple alphabets by running the script multiple times with different labels.

The script will capture frames as you press the 's' key and save them to a data folder with the label as the subdirectory name.  


## Model Training
After collecting data, you can train the model using Google's Teachable Machine.

Go to Teachable Machine and create a new project.

Upload the data for each alphabet (A, B, C) to the corresponding class.

Train the model using the "Train" button.

Download the TensorFlow model (a .h5 file) and save it to the model folder.

## Testing
The test_model.py script allows you to test the trained model using your webcam.

To test the model, run the following command:  
`python test.py`  

The script will display the webcam feed with the predicted alphabet label overlaid on top of the hand region.

## Conclusion
This project demonstrates how computer vision and machine learning can be used to recognize American Sign Language alphabets in real-time using a webcam. The trained model can be used to build more advanced applications such as ASL translators and communication aids.
`
