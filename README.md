# Saliency-Maps
**Generation of Saliency Maps Using Neural Networks**

The Human eyes automatically focus on the most attractive regions. This is a naturally
occurring event. It is complicated to make the computer imitate the way the human eye
does while seeing an image. One of the methods to achieve this is by training a neural
network with a sufficient amount of dataset.
Saliency Maps define each pixel's unique quality. It is the representation of the Image in
a unique manner that is easier to analyze and is also meaningful. It is an image in the form of a map where people are expected
to look irrespective of the task they are doing. Saliency Maps are usually rendered as
a heatmap. The hotness in the heatmap refers to the region of interest, whereas the
Saliency Maps refers to the probability of each pixel.

**Proposed Implementation**

![BlockDiagram](https://user-images.githubusercontent.com/63425115/103107126-b7775d00-463b-11eb-85f0-c5936938af5e.JPG)
The input image and its ground truth will act as the input to the neural network. The
dimensions of input image, ground truth are 512x512x3 and 512x512x1 respectively. The
enocder-decoder of the neural network processes this data and outputs a saliency map
with a dimension 512x512x1. The pre-trained model used in the project is ResNet-50. It
is not possible to achieve the desired result by using ResNet-50 alone. So, the need for
modications in the pre-trained model is essential, we consider
the ResNet-50 as the encoder and the modifications added to it will be the decoder.