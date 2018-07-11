# Problem Statement

I have this kinds of images:


Key Point: I have texture-less, mostly monochromatic T-shirts, which is of great importance in using color based segmentation & thresholding.

Dataset comprises of 350[2-3 Tshirts] + 2000[5-6Tshirts]
D1 + D2

For each image, I would like to generate N masks, one each for every T shirt, and 1 for BG. 

I will choose a HSV thresholds of max and min therefore 6 values for each mask(each T shirt color)  to be generated.

But before all this, I came across Otsu's method and Image quantization , so should check that too.

# Approaches

I have tried different algorithms and this is my survey repository, to store the results I was getting and finally getting the required output.

# Current Directory structure [excluding files]
```
.
├── 2TC
├── 2TD
├── 2TP
├── 3T
├── capture
└── samples
```



Hurdles
1. How to evaluate accuracy/ generalizability of this method ?
2. This data will actually go into a segmentation neural network to train, then why am I using Neural net again ?
[Because I'm hoping that with batch normalization, the neural network will generalize enough to overcome the color specificness and heruristics ? ]
