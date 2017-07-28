
Description: use Fully Convolutional Network to segment road (drivable regions) and lane marks for self driving.

<a href="https://youtu.be/xwhcjtnm1JQ" rel="some text"><p align="center">![Foo](https://j.gifs.com/O7mK6E.gif)</p></a>

The network was trained on the huge segmentation datasets for future maps provided by Mapillary. The testing videos are a random dashcam video on Youtube. The result for road segmentation is highly accurate but the result for lane mark segmentation is a lot less accurate. However, it is still good enough to estimate the rough positions of the lanes.

Thanks to https://github.com/JihongJu/keras-fcn and https://www.mapillary.com/.

# To do list

1. More advanced post processing using Edge Detection.
2. Fine tune the segmentation result using Dilated Net or SegNet with Conditional Random Field.
3. Additionally trains on CamVid dataset and SYNTHIA dataset.

# Usage

1. Download the data from https://www.mapillary.com/ (need to make a request) or download the pretrained weights from https://goo.gl/cnUCzv.
2. Follow the instructions in Lane Detection.ipynb to construct and train the network for road and lane mark segmentation on random dashcam video.
