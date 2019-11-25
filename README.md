# Image Processing Project
## Project Name: Traffic sign recognition method for intelligent vehicles
This project implements a new approach for traffic sign recognition, the image pre-processing approach is referenced from the paper ['Traffic sign recognition method for intelligent vehicles'](https://www.researchgate.net/publication/328418844_Traffic_sign_recognition_method_for_intelligent_vehicles), SVM classifiers and MLP classifiers are used to compare the performance.
## Proposed Method
![Alt text](https://github.com/suinaowawa/Image-Processing-Project/blob/master/figures/1.PNG)
The process has three steps. 
1. Transform the image from the Cartesian coordinate system to the log-polar one with post-processing. 
2. Feature extraction, histogram of oriented gradients (HOG) and local binary pattern (LBP) are used to represent the image in the log-polar coordinate system. 
3. Classification using support vector machines (SVM) and multilayer perceptron (MLP) classifiers.

## Performance analysis
1.	Cartesian vs. Log-polar

First, we test the performance of cartesian and log-polar transform on combining features using the SVM classifiers.
![Alt text](https://github.com/suinaowawa/Image-Processing-Project/blob/master/figures/result1.PNG)
From the result, we can see that log-polar transform improves the accuracy.

2.	HOG, LBP and Combining features

Then, we make comparison between different feature extraction. The tests are run on SVM classifiers with log-polar transformation step.
![Alt text](https://github.com/suinaowawa/Image-Processing-Project/blob/master/figures/result2.PNG)
From the result, we can see that by combining feature of HOG+LBP, we enhance the performance.

3.	SVM classifier vs. MLP classifier

The following tests are run on combining feature extraction with log-polar transformation.
![Alt text](https://github.com/suinaowawa/Image-Processing-Project/blob/master/figures/result3.PNG)
From the results above we can see that, both two classifiers have good performance,
SVM have a better accuracy while MLP is faster in terms of recognition speed as well as the training speed.

In a word, the proposed method of have a good performance in terms of time and accuracy. It is feasible to implement in a simple, low-cost application.
