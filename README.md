# FFCR-Final Repository
 
The **Forensic Facial Sketch Construction and Recognition (FFCR)** project is a deep learning–based system designed to construct facial sketches from images and recognize individuals by analyzing visual facial features. The system integrates image processing, machine learning techniques, and a web-based interface to provide an interactive platform for facial recognition and identification.

The architecture of the system consists of two main components:
 - Backend processing for image analysis and recognition
 - A frontend interface that allows users to interact with the system and visualize results.

This repository contains the complete source code and assets for the Final Year Project titled **Forensic Facial Sketch Construction and Recognition (FFCR)**.

## Repository Structure

The repository is organized into the following main directories and files:

- **[Backend](#backend)**
- **[Desktop](#desktop)**
- **[Other Python Scripts](#other-python-scripts)**
- **[FFCR.persons.json](#ffcrpersonsjson)**
- **[test_DataSet_Summary.txt](#test_datasetsummarytxt)**
- **[Trainin_DataSet_Summary.txt](#trainin_datasetsummarytxt)**
- **.gitignore**

---

### Backend

The `Backend` folder contains all the necessary files for the server-side of the application. It includes scripts for handling image processing, facial recognition, and interaction with the database (MongoDB).

Key components:

- **Flask Server**: Handles HTTP requests, image uploads, and responses.
- **Image Processing Scripts**: Python-based scripts process input images and perform operations      such as:
  - Feature extraction
  - Sketch generation
  - Facial recognition
- **Database Management**: Interacts with MongoDB to store and retrieve recognized person details.

### Desktop

The `Desktop` folder houses the frontend part of the application, which serves as the user interface for interacting with the FFCR system. This includes the following:

- **User Interface**: Allows users to upload images, capture images via webcam, and display recognition results.
- **Integration with Backend**: Sends images to the backend for processing and displays the results received from the server.
- **Assets**: Contains images, icons, and other static resources used in the UI.

### Other Python Scripts

This directory includes various utility scripts used for preprocessing the dataset and summarizing data:

1. **processDataSet.py**:

   - Converts facial images to sketches.
   - Applies enhancement techniques like contrast adjustment.
   - Saves both the original and processed images.

2. **resize.py**:

   - Resizes images to a standard dimension required for the training models.
   - Ensures consistency in input data for better accuracy in recognition.

3. **summarizeDataSet.py**:
   - Generates a summary report of the dataset.
   - Counts the number of images and categorizes them by type (original, sketch, etc.).

### FFCR.persons.json

This JSON file contains structured data intended for MongoDB. It includes details about the persons in the dataset, which are used during the recognition process to identify and match images. This file serves as a schema for the database.

### test_DataSet_Summary.txt

A text file that provides a summary of the test dataset. It includes information such as:

- **Number of Images**: Total count of images available

### Trainin_DataSet_Summary.txt

Similar to the `test_DataSet_Summary.txt`, this file summarizes the training dataset used for model training. It contains:

- **Total Image Count**: Number of images used for training.

### Technologies Used
 - Python
 - Flask
 - MongoDB
 - Deep Learning libraries for facial recognition

### Applications
The FFCR system demonstrates potential applications in:
  - Forensic investigations
  - Identity verification systems
  - Security and surveillance technologies

### .gitignore

The `.gitignore` file specifies the files and directories that should be ignored by version control to maintain a clean repository. This typically includes:
 - temporary files
 - system-generated files
 - cached datasets
   
This helps maintain a clean repository.

---
