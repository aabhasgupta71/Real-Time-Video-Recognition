# Real-Time-Video-Recognition
This is a real time video recognition system which uses KNN algorithm for classification/recognition and Haarcascade classifier for facial detection.
The description of the various files/folders are as follows:
- **face_data_collect.py** -> This is a python file which is used for generating training set data using live feed frames captured through webcam and stored in the form of numpy arrays indexed with the name of the person. The default path for dataset to be stored is set to './data'.
- **face_recognition.py** -> This is a python file which is the heart of the process of facial recognition. It uses Haarcascade classifier for facial detection and KNN algorithm for classification/recognition. 
- **data** -> This is the folder which stores numpy arrays corresponding to images indexed using person names and the files stored in this folder are of the form '.npy'.
- **Haarcascade** -> This is the folder which contains the XML file for haarcascade classifier.

### Instructions

- Clone the repository and navigate to the downloaded folder.
- Type the command ```python face_data_collect.py```.
- The prompt asks the name of the person for which data is being collected. Enter the name of the person and press Enter. The process of collection of frames via webcam feed starts. Press 'q' on the keyboard to stop the process.
- The numpy array of the person is stored in the "data" folder. Do the same for all the people you wish to make a dataset for.
- At last type ```python face_recognition.py``` on cmd. The process of recognition starts and the person's name is displayed on the camera feed using OpenCV.
