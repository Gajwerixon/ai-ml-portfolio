# Project Summary

This project focuses on **road sign detection using YOLO (You Only Look Once)**. The goal was to train an object detection model capable of detecting and classifying different types of road signs in images.

The dataset contained images and corresponding annotations stored in **XML format**. During data preprocessing, the XML annotations were inspected and converted into the YOLO format, where each object is represented by its class ID, bounding box center coordinates, width, and height. The bounding box coordinates were normalized to make them independent of the original image dimensions.

The dataset was then divided into training and validation sets, and a `data.yaml` file was created to provide YOLO with information about the dataset and available classes.

A pretrained **YOLO26n** model was fine-tuned on the prepared road sign dataset. Model performance was evaluated using **Precision, Recall, mAP50, and mAP50-95**. The training results showed that the model improved during the first part of training, while the main metrics became relatively stable in the later epochs. Early stopping was used to prevent unnecessary training once the validation performance stopped improving.

Finally, the trained model was tested on images from the validation set. The model was able to detect most road signs correctly, although some objects were still missed in certain images. This visual evaluation helped identify cases where the model could be improved further.