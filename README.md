# Intelligent Document Processing System for ID Cards
This repository is about implementing an ID Card Data Extraction system that automates the process of extracting key information from ID cards using a combination of object detection and Optical Character Recognition (OCR). The extracted data will be store to a NoSQL database, MongoDB Atlas.

## Features

* **Object Detection:** Accurately detects and locates relevant fields on an ID card (e.g., name, ID number, date of birth) using a custom trained model with YOLOV9c.
* **OCR:** Extracts text from the detected fields using the Google Vision API.
* **Data Storage:** Stores the extracted data in a MongoDB database for easy access and management.

## Technologies Used

* **Programming Language:** Python
* **Object Detection:** YOLOV9c from Ultralytics
* **OCR:** Google Vision API
* **Database:** MongoDB Atlas (Saas Platform)

## How it Works

1. **Input:** The system takes an image of an ID card as input.
2. **Object Detection:** An object detection model is used to identify and locate specific fields on the ID card. These fields likely include areas like the name, date of birth, ID number, and photo. 
3. **Image Analysis and Object Detection:** This step involves further analysis of the detected fields, potentially including image preprocessing or enhancement to improve the accuracy of the subsequent OCR.
4. **Google Vision API (OCR):**  The Google Vision API is used to perform OCR on the detected fields. This converts the text within those fields from an image format into machine-readable text data.
5. **Data Storage:** The extracted text data (decoded by the OCR) is then stored in a MongoDB database in the cloud.

## System Pipeline
![id_card_procesing_system_pipeline](https://github.com/user-attachments/assets/868b10ca-2662-4381-85cb-d7c40bbb6929)

## Training Result
![id_card_training](https://github.com/user-attachments/assets/d256d592-ceb3-407d-ba20-7933835c3827)

## Inference Result
![id_card_prediction](https://github.com/user-attachments/assets/997fd588-f894-4fbc-b2f5-59e5cc0f1e64)

Did you find this project useful?  I'd be thrilled if you could give it a star ⭐ and follow me to stay updated on my latest work!  Thanks for your support! 😊
