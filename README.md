# Automatic-Disc-Herniation-Segmentation-and-Classification
Automatic Disc Herniation Segmentation and Classification Using Deep Learning Models on Lumbar Spine Magnetic Resonance Images

README.txt

MSC. APPLIED DATA SCIENCE WITH ADVANCED PRACTICE PROJECT

Automatic Disc Herniation Segmentation and Classification Using Deep Learning Models on Lumbar Spine Magnetic Resonance Images



##########
Information.  
##########
The files contained in this .zip were created as part of the desertion submission for the module ‘computing masters project’ of the course ‘MSc Applied Data Science with advanced practice’ (May 2023) at Teesside University. 

Author: AGUAGWA EMMANUEL UCHENNA
Email: Emmanuel96uc@yahoo.com

##########
Background
##########

Disc herniation is a common spinal disorder that can cause back pain and other related symptoms. Accurate diagnosis and treatment of disc herniation are critical for patients' quality of life. However, manual diagnosis of disc herniation can be time-consuming and subject to inter-observer variability. Therefore, the development of an automated tool that can accurately segment and classify disc herniations can greatly assist medical professionals in the diagnosis and treatment of this condition.



##############
Installation and requirements 
##############
To use this project, you need to install the required dependencies. You can do this by running the following command:

pip install -r requirements.txt


#####
Usage
#####
To use the model for disc herniation segmentation and classification, you need to:

first, run the 
data_preprocessing_UNET.ipynb file

•	In this script, we downloaded data from the above link and unzipped files to create the desired data set.
•	The images were then resized, and the data set was divided into train and test sets.
•	Data was saved for the next steps.

Next, you run 
train_model_UNET.ipynb file
•	In this script, we trained a UNET model to extract the region of interest (ROI) from MR images.
•	Model was saved for the next steps.


Next, you run
ROI_UNET.ipynb file
•	In this script, we loaded the pre-trained model and extract ROI from the full data set.
•	Then saved the extracted ROI images for the next steps.


Next, you run

data_enhancement.ipynb file
•	In this script, we did image enhancement to get better images.
•	Then saved images as numpy files.

Finally, you run

image_classification.ipynb file

•	In this script, we downloaded the radiologist report and ground truth dataset.
•	After that, load data and perform image augmentation to increase data variation.
•	Finally we trained a CNN classification model on the data.



####
Data
####

The datasets used for this project are linked bellow

link to the dataset
https://data.mendeley.com/datasets/k57fr854j2/2

link to the ground truth dataset
https://data.mendeley.com/datasets/zbf6b4pttk/2

link to radiologist report for lumbar spine medical resonance image dataset
https://data.mendeley.com/datasets/s6bgczr8s2/2

#####
Tests
#####
This project was hosted on google drive and executed using Google Collab. The link to
accessing the project on the server can be found below.
https://drive.google.com/drive/u/1/folders/169Dn_rdx51oHsBw1xnXxd4j4WMotqoVO

#############
Acknowledgements. 
##############
My deepest appreciation goes out to everyone who helped bring this project to fruition.
To begin, I want to acknowledge the blessings and guidance of God Almighty who kept me
alive and healthy throughout my stay in the university and through this dissertation.
I would like to express my sincere appreciation to my family and friends for helping me through
this project in one way or the other. Their support and understanding were very important in
helping me stay focused and driven.
To my supervisor, Ala AL Kafri who paid close attention to details to make sure I got off on
the right foot in this project. The weekly presentations kept me up and going.
Additionally, I would like to thank the faculty and staff of the School of Computing,
Engineering, and Digital Technologies, Department of Computing and Games, Teesside
University for its academic and administrative support, which helped me to navigate the
challenges of the dissertation process.
A heartfelt "thank you" is in order to everyone who contributed to the success of this
dissertation. I appreciate all of the help, motivation, and encouragement you gave me.



Thanks again!


#########
License
#########

MIT License

Copyright (c) [2023] [AGUAGWA EMMANUEL UCHENNA]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.



