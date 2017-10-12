## Project Semantic Segmentation
![](http://om1hdizoc.bkt.clouddn.com/17-8-27/87401135.jpg)
### Intro
This project is to implement a FCN-8 network. Instead of starting from the beginning. We are asked to take advantage of the already implemented VGG-16 architecture. We use the VGG-16 as encoder and build decoder from it. The goal of this FCN-8 is to highlight where free-space are in a picture in green.
### Things used
#### 1x1 convolution
The 1x1 convolution connect layer7 of the VGG-16 and preserve space information via 4-D representation.
#### Upsampling
The upsampling convolution restore the shrinked image back to the original one. There are three layer of upsampling layer.
#### Skip layer
The skip layer are used so the deep neural network see things from the whole picture. There were two of them.
### Parameters
I set total epoch for training as 15. The learning rate as 0.001. The batch size to be 4. The optimizer as Adam. 
### Conclusion
Overall this is a fun project to work with. Except I have to spend money on AMIs. The challenges mostly come from not understanding what the code does at the very beginning. Somehow I have to manually download the VGG model instead of downloading it on the terminal.