# CS_SOP
## Caution Board Detection System for Visually Impaired
This repository contains the code and data for a caution board detection system designed specifically for visually impaired individuals. The system utilizes YOLOv5, a state-of-the-art object detection algorithm, fine-tuned on a custom dataset to detect caution boards in real-time.

## Project Overview
The aim of this project is to assist visually impaired individuals in navigating their surroundings safely by detecting caution boards and providing audio or haptic feedback to alert them of potential hazards. By leveraging computer vision technology, we strive to enhance the independence and safety of visually impaired individuals in various environments.

## Dataset Structure
The data.zip file included in this repository contains the dataset used for training and evaluation of the caution board detection model. Below is the structure of the data.zip file:

data.zip <br />
│ <br />
├── images <br />
│   ├── train <br />
│   └── val <br />
│ <br />
└── labels <br />
    ├── train <br />
    └── val <br />

images: Contains the image data used for training and validation. The train and val folders respectively contain the training and validation images.

labels: Contains the corresponding annotation labels for the images. Similar to the images folder, the train and val folders hold the training and validation annotation files.

## Usage
### Clone Repository: Clone this repository to your local machine.
### Extract Data: Extract the data.zip file to access the dataset
### Train Model: To train the YOLOv5 model on the provided dataset, use the following command:
!python train.py --img 640 --batch 2 --epochs 60 --data data.yaml --weights yolov5s.pt --cache
Evaluate Model: Evaluate the trained model on the validation set to assess its performance. Utilize the evaluation scripts provided in the repository.
