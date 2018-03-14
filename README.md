## Vehicle Detection and Tracking
In this project I have used a image processing using OpenCV and machine learning from scikitlearn library to detect cars in an image taken from a camera mounted in the front of a car.

First of all I started with finalizing the features that I needed to use for this project. I have used Histogram of Oriented gradients for this project. I trained a linear SVM classifier to find out if an image is car or not a car. The training examples were frim GIT database and they are 64x64 RGB images. Here is the link for the training examples:
https://www.gti.ssr.upm.es/data/Vehicle_database.html

Then I used sliding windows technique to detect an image in piecewise manner. The size of the window was different depending upon where I was looking for the cars. After that I used heatmap and heatmap threshold to get rid of false positives from the images. Then I ran the algorithm on a video and after running it ona  video I also considered deteccted cars in the last 15 frames to give more rhobust results.

Here is a video output showing detected cars in a video:
[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/_6v5DhuVh3U/0.jpg)](https://www.youtube.com/watch?v=_6v5DhuVh3U)