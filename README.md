# Object Detection on Aerial Video Footage

This repository contains code and documentation for our deep learning assignment on object detection of airplanes, birds, drones, and helicopters in aerial video footage. The goal of this assignment was to train a model to perform object detection and plot down the boundary boxes for each object detected.

## Dataset

We used a batch of video footage of skies as our dataset. To match with the number of rows provided in the CSV file containing the boundary box coordinates and class of objects detected, we converted the videos to frames at a rate of 29.96 fps. The dataset included various types of objects, such as airplanes, birds, drones, and helicopters. After conversion to frames, we were left with a huge dataset of almost 90k images, from just 280 videos.

## Approach

To accomplish our task, we used PyTorch implementation of Faster R-CNN for object detection. Faster R-CNN is a popular and effective algorithm for object detection that uses a region proposal network (RPN) to generate object proposals, and a second stage network to refine the proposals and classify them into different categories.

We split our dataset into training and validation sets, with 80% of the data used for training and 20% for validation. We trained our model using a learning rate of 0.001, a batch size of 10, and the Adam optimizer. After training our model for 1 epoch, we achieved an accuracy of 89% on our Validation set.

## Results

Our trained model was able to detect airplanes, birds, drones, and helicopters in aerial video footage with high precision and recall. We visualized the object detections by plotting down the boundary boxes for each object detected.

## Conclusion

Object detection is a critical task in computer vision and has various real-world applications. In this assignment, we demonstrated how to perform object detection on aerial video footage using PyTorch implementation of Faster R-CNN. We achieved high accuracy and visualized the results by plotting down the boundary boxes.

