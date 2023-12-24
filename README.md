# Deep Learning Basics

This repository houses select assignments from the Deep Learning course at my UCLA Master's in Business Analytics program. The course was taught by Danylo Vashchilenko (https://github.com/hellodanylo/ucla-deeplearning).

## Autoencoder
MNIST images were intentionally subjected to random noise, and an autoencoder was used to remove noise, aiming to minimize the difference between the Denoised and Clean images. I was able to achieve an MSE between Denoised and Clean images of < 0.02 on the scoring set.

## RNN
Both LTSM and GRU cell types were used to forecast temperature across 30+ cities based on past temperature, humidity, pressure, and wind speed. Additional temporal features such as months and seasons were added to assess model performance. An R squared of > 0.85 was achieved by using a LTSM model on the scoring set.

## Ensemble
I used multiple object detection models to count vehicles and signal objects in images. I tried heuristic methods and a blender model using predictions from these detectors. While experimenting with transfer learning from ResNet50 and InceptionV3, I found their MSE was not lower than any object detection models. By taking the highest prediction among all detectors with a confidence threshold at 43%, I was able to achieve the lowest MSE among all submissions in the class.
