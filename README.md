# Sign_language_detector

This Python project utilizes computer vision and machine learning to detect and recognize American Sign Language (ASL) alphabets A, B, and C in real-time through the webcam.

![ASL](https://user-images.githubusercontent.com/116836999/225982125-a558929a-599b-4d67-bc83-0b43018088d3.png)


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
`python dataCollection.py`  

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


## Results

![A](https://user-images.githubusercontent.com/116836999/225985536-05bffc4a-a611-4127-98fb-c0136d22c31d.png)
![B](https://user-images.githubusercontent.com/116836999/225985571-76d3ba23-f6f1-4fa0-8867-da8380951205.png)
![C](https://user-images.githubusercontent.com/116836999/225985616-4f6beba7-1a41-4dd9-a0dc-8c619a59bc40.png)


## Conclusion
This project demonstrates how computer vision and machine learning can be used to recognize American Sign Language alphabets in real-time using a webcam. The trained model can be used to build more advanced applications such as ASL translators and communication aids.
`
