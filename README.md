# Real-time-Number-Plate-Recognition-System-using-YOLO-EasyOCR-Sort
This project is a real-time Number plate Recognition System designed to identify and read vehicle license plates using advanced computer vision techniques. The system utilizes a combination of YOLOv8, EasyOCR, and Sort to detect and track vehicles and read their license plates.

## Dataset
The [dataset](https://universe.roboflow.com/roboflow-universe-projects/license-plate-recognition-rxg4e) includes 24242 images.
License plates are annotated in YOLOv8 format.

## Models
A **YOLOv8 pre-trained model** to accurately detect vehicles in video feeds.

Utilizes a **specialized license plate detector model**, trained with YOLOv8 using above dataset, to detect license plates on detected vehicles.

## Dependencies
  1. **EasyOCR**: Used for Optical Character Recognition (OCR) to read the text on the license plates
  2. [**sort**](https://github.com/abewley/sort): A module used for tracking vehicles, ensuring each detected vehicle is followed consistently across frames.

## Repository Structure
  1. **main.py**: The core script that processes the video feed, orchestrates the vehicle and license plate detection, and manages tracking. It integrates all components to output real-time results.
  2. **util.py**: Contains auxiliary functions essential for the system’s operation. These include functions for tracking vehicles, identifying license plates, reading the number plates, and verifying the format of the number plates.
  3. **model_train.ipynb** - Script to train license plate detector model
