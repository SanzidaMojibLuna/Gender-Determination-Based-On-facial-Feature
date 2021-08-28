This project is about gender detection from image.

CNN model is used as the main training tool. The CNN model has 3 convulation layers
and 2 fully connected layers. 

Conv1 : The first convolutional layer has 96 nodes of kernel size 7.
Conv2 : The second conv layer has 256 nodes with kernel size 5.
Conv3 : The third conv layer has 384 nodes with kernel size 3.
The two fully connected layers have 512 nodes each.

new_model.py is the runnable python file. There are other 4 files:
1.opencv_face_detector.pbtxt
2.opencv_face_detector_uint8.pb
3.gender_deploy.prototxt
4.gender_net.caffemodel

These are weights and model for face and gender detection and needsto be 
in the same folder as the source code. 

The images from which gender needs to be detected has to be in the 
same folder too. A good number of sample image for testing out the 
source code is also given here. Image can be in jpg, jpeg or png form.

For running the source code the following command should be given in the 
command propmt :
python new_model.py --input <image file name with extension>