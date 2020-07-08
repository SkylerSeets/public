# EXERCISE 1
## The output is a list of numbers. Why do you think this is, and what do those numbers represent?
The numbers represent the percentage that each neuron returns of its confidence that the input is a certain number. The highest number represents the overall network's guess on what the number is with the given input. 

## What does this list represent?
The list represents 3. The probability that this item is in each of the 10 classes (the 0-9 digits)

## How do you know that this list tells you that the item is an ankle boot?
I know this because 2. The 10th element on the list is the biggest, and the ankle boot is labeled 9. It should be noted that the 10th element is actually the digit 9 which represents the ankle boot since the neurons are numbered 0-9 for a length of 10. 

# EXERCISE 2
## Experiment with different values for the dense layer with 512 neurons. What different results do you get for the loss, training time, etc.? Why do you think that's the case?
For a dense layer of 512, I get a loss of 0.2800 and a total training time of 30s. For a dense layer of 256, I get a loss of 0.2857 and a total training time of 20s. For a dense layer of 128, I get a loss of 0.2941 and a total training time of 15s. It takes time to calculate the loss and optimize the network. I believe that this is taking the most time and that is causing both the decrease in loss and the increase in time as the number of neurons in the dense layer increases.

## Increase to 1024 Neurons -- What's the impact?
1. Training takes longer, but is more accurate. The dense layer of 1024 returns a loss of 0.2792 and a total training time of 55s compared to the dense layer of loss 0.2800 and 30s respecively. 

# EXERCISE 3
## What would happen if you remove the Flatten() layer. Why do you think that's the case?
I get a ShapeError. This is because our data is currently 28x28 pixel images, and we cannot have a 2D network. We need to flatten the 2D array into a 784 1D array for the model to work. 

# EXERCISE 4
## Consider the final (output) layers. Why are there 10 of them? What would happen if you had a different amount than 10? For example, try training the network with 5.
There are 10 neurons to match the 10 expected outputs for the network. I get a InvalidArgumentError when I try training the network with 5 instead of 10 neurons in my last Dense layer. 

# EXERCISE 5
## What would happen if you add another layer between the one with 512 and the final layer with 10?
There is not a large impact. The loss is 0.2775 and takes 45s to train. The accuracy is better by about .025 and takes about 15s longer compared to a single Dense layer of 512.

# EXERCISE 6
## Consider the impact of training for more or less epochs. Why do you think that would be the case?
The more epochs you train, the higher the accuracy. This is because the epochs is how many times the optimizer is able to run, or how many times the network itself is trained. So the more times you train the network per run, the better its accuracy due to the optimizer optimizing the network.

# EXERCISE 7
## Before you trained, you normalized the data, going from values that were 0-255 to values that were 0-1. What would be the impact of removing that? Here's the complete code to give it a try. Why do you think you get different results? 
The impact could be that some neurons are used more and therefore have a greater impact on the overall network when calculating the probabilites of the output.

# EXERCISE 8
