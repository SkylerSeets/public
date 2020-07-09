# A
The data is split into training and testing data to minimize the network's ability to memorize the dataset and return an overfit model. By splitting the model into a training and testing set, we give the computer one set of data to fit on, and test it using another set of data. In this way, the network that memorizes the overall noise and pattern of the training data will fail on the never before seen testing data. In this way, you can be guaranteed a model that actually relates the data by rules instead of a model that memorized the data. 

# B
https://www.kaggle.com/dansbecker/rectified-linear-units-relu-in-deep-learning

The .relu function, also know Rectified Linear Units, is a function that takes all negative inputs and instead returns 0. So for example, if there are two inputs A and B and their relation is f(2A + 2B), and A=1 and B=1, then the .reflu function would return 4. However, say B=-1, then the function would return 2. Instead, if B=-100, then the function would return 0. For the .softmax function, the funciton takes the largest number in the array and sets that as 1 while setting all the others as 0. This then makes searching for the output easy since the computer only has to look for the 1 instead of the max of the outputs, saving time and memory. 

We feed the computer a handwritten digit in grayscale and standardized and the computer returns what it thinks the digit is. Since there 10 digits that can be fed into the computer (0-9), we need 10 neurons in the third layer to capture all the possible outputs that we can have (0-9). 

# C
The loss function calculates the total loss, the deviation from the expected result using the model's output. The optimizer then takes the computed loss and uses that to optimize the model. This is done over many times, each time optimizing the model in order to get a best estimate over each iteration.

# D
1. There are 60,000 images that are (28,28) pixels.
2. There are 60,000 labels.
3. There are 10,000 images that are (28,28) pixels.
4. Private Code
5. Private Code
6. Private Code
