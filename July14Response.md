# QUESTION 1
![Original Image](https://raw.githubusercontent.com/ashuang2013/public/master/OriginalImage.png) <br/>
This is the original image taken from the scipy library

![Sharpen Image Filter](https://raw.githubusercontent.com/ashuang2013/public/master/SharpenFilterConv.png) <br/>
Applying the filter [[0, -1, 0], [-1, 5, -1], [0, -1, 0]] sharpens the image. When performing a convolution on an image, the computer takes a singular pixel and applies the entire filter to the pixel's corresponding neighbors. Take for example this pixel in grayscale with value 192: <br/>
| 0 | 64|128|
|---|---|---|
| 48|192|144|
|142|226|168|

The filter is then applied where each pixel is multiplied by its respective pixel in the filter and then added together. For example, this convolution would produce <br/>
(0x0) + (-1x64) + (0x128) + (-1x48) + (5x192) + (-1x144) + (0x142) + (-1x226) + (0x168). <br/> <br/> This would then be the new value for the pixel in grayscale that had value 192.
However, since there is no 3x3 square in the corners, the computer is unable to perform the convolution. Therefore, both the vertical and horizontal edges would be cut out of the convoluted image. With one pixel cut in each dimension, the convoluted image would diminish in size, 2 pixels overall. So a 28x28 image after convolution would become 26x26.

These are some other filters along with their images: <br/>
Blur Image Filter: <br/>
![Blur Image Filter](https://raw.githubusercontent.com/ashuang2013/public/master/BlurFilterConv.png)  <br/>
Edge Filter: <br/>
![Edge Filter](https://raw.githubusercontent.com/ashuang2013/public/master/EdgeFilterConv.png)

*What this functionally accomplishes is the ability*

This is important in computer vision because computers themselves cannot take an image and then say, sharpen the image. However, the computer can manipulate numbers, and through the manipulation of numbers in the shape of a 3x3 matrix we can create what we want (sharpening the image). 
