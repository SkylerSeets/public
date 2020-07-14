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

*What this functionally accomplishing is using a 3x3 matrix called the filter and applies it to every pixel in the image and changes the image (see above).*

This is important in computer vision because computers themselves cannot take an image and then say, sharpen the image. However, the computer can manipulate numbers, and through the manipulation of numbers in the shape of a 3x3 matrix we can create what we want (sharpening the image). 

# QUESTION 2
Through pooling, I have managed to halve the number of pixels in the image from 512 to 256. The pooling filter used is MAX pooling. Looking at the code, you see that it iterates through the entire 2D image and creates a list called pixels. Then it takes the 2x2 square from the current iterated pixel much like convolutions and then takes those pixel values. It then sorts the pixels in reverse (descending) order and then takes the value at cell 0 and inserts it into the newImage created at the beginning with half the dimensions of the original image. <br/><br/>
The reason that this is MAX pooling is because since the pixel values are sorted in descending order, we would have the largest values at the beginning of the list and the smallest values at the end. Since we are taking the pixel value at index 0, we are taking the largest value in that sorted array, also known as the max value in that array, hence MAX pooling. <br/><br/>
Again, since we are halving the overall picture by applying a 2x2 filter that only takes the max pixel value in the 2x2 matrix, we will have a reduction in the size of the image. This method is useful because it saves time by cutting down the steps needed to process an image (think processing 512x512 pixels vs 256x256 pixels, a 4x reduction). Not only that, but it helps to reshape images into another size (taking the same example, if I need a 256x256 pixel image but I have a 512x512 pixel image, I can just halve its dimensions using MAX pooling). The _most_ important aspect to pooling however, is that it retains the important information even while being compressed. 
![Pooled Image with Edge Filter](https://raw.githubusercontent.com/ashuang2013/public/master/PooledEdgeFilterConv.png) <br/><br/>
This image has been pooled from the original image in Question 1 that has been convoluted with the Edge Filter. Notice that the image length has been halved from 512x512 pixels to 256x256 pixels. However, notice that the image did not change too much, and still retains the important edge filter from the original image. 

# QUESTION 3
The lecture for today (Coding with Convolutional Neural Network) compared the 
application of our previously specified deep neural network with a newly specified 
convolutional neural network.  Instead of using the fashion_MNIST dataset, use the 
mnist dataset (the hand written letters) to train and compare your DNN and CNN output.      
Were you able to improve your model by adding the Conv2D and MaxPooling2D layers 
to your neural network?  Plot the convolutions graphically, include them in your 
response and describe them.  Edit the convolutions be changing the 32s to either 16 or 
64 and describe what impact this had on accuracy and training time.  What happens if 
you add more convolution layers? 
