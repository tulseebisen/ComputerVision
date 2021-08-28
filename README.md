# ComputerVision

## Image Background Removal

### It’s a common practice now a day to replace existing background from a photo or video with nicer image or another video. There are a number of Deep Learning algorithms works which detects a solid colored background thereby removes it from the photo or video. The other option is masking of the background that we want to remove.

Oe another method is image segmentation , Image segmentation has a lot of amazing applications that solve different computer vision problems. PixelLib is a library created to ensure easy integration of image segmentation in real life applications.

We can also use U-Net, two different classification models, VGG16 and ResNet34 or combination of them or ,MODNet(matting method) also

#### Here I have used two methods :
1) PixelLib with Deeplabv3 pretrained model: which uses Image Segmentation

The key role of image segmentation is to remove the objects segmented from the image and place them in the new background created. This is done by producing a mask for the image and combining it with the modified background. We make use of deeplabv3+ model trained on pascalvoc dataset. The model supports 20 common object categories, which means you can change the background of these objects in images.

**download the pre-trained model:** 

(Open your browser and copy this URL there, press enter) [https://github.com/ayoolaolafenwa/PixelLib/releases/download/1.1/deeplabv3_xception_tf_dim_ordering_tf_kernels.h5]

**2) Masking with Threshold** 
In this process I am doing using threshold to create mask and then background is chaged according to requirement.

### Expected Output
![view_Output_Expected](https://user-images.githubusercontent.com/79663448/131219076-9b17f4ed-13e5-42df-a946-9dd318cdea81.jpeg)
### Input
![view1](https://user-images.githubusercontent.com/79663448/131219079-340db05e-eea7-43f4-8dd8-274779bf1e75.jpeg)

Author:
Tulsee Bisen


