
Description: use Fully Convolutional Network to segment road (drivable regions) and lane marks for self driving.

<a href="https://www.youtube.com/watch?v=dgP7nEaEkKs&feature=youtu.be" rel="some text"><p align="center">![Foo](https://j.gifs.com/nZ2R0D.gif)</p></a>

The network was trained on the huge segmentation datasets for future maps provided by Mapillary. The testing video is a random video on Youtube. The result for road segmentation is highly accurate but the result for lane mark segmentation is a lot less accurate. However, it is still accurate enough to estimate the rough positions of the lanes.

Thanks to https://github.com/JihongJu/keras-fcn and https://www.mapillary.com/.

# To do list
1. Fine tune the segmentation result using Dilated Net or SegNet with Conditional Random Field.
3. More advanced post processing using Edge Detection.
2. Additionally trains on CamVid dataset and SYNTHIA dataset.

# Usage

1. Lane Detection.ipynb => contains instructions to construct and train the network for road and lane mark segmentation on random dashcam video.
