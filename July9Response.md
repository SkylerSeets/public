# QUESTION 1
According to the TensorFlow website (https://www.tensorflow.org/hub/overview), TensorFlow Hub is a "repository and library for reusable machine learning. The tfhub.dev repository provides many pre-trained models: text embeddings, image classification models, and more." Basically, its a library like sklearn that has many useful tools related to machine learning. 
We used TensorFlow Hub to import the IMBD datasets which contains the movie reviews training and testing sets and the embedding model that "maps a sentence into its embedding vector" (https://www.tensorflow.org/tutorials/keras/text_classification).

# QUESTION 2
The optimizer is how the model "learns" and the loss function tells the optimizer how to improve. The loss function makes a certain computation (can be based on many different functions, for example "BinaryCrossentropy" or "Mean Squared Error" that tells the optimizer how far away it is from the correct answer. The optimizer then optimizes based on the loss function and once again tests the model. This then happens over the epochs, each time the model calculating the loss and the optimizer optimizing the model. 
The model had an accuracy of .9519 and a loss of .1465 after 30 epochs for the training data. The model had an accuracy of .863 and a loss of .3063 for the testing data. The model is definitely overfit.

# QUESTION 3
![Training and Validation Graph](/public/Training and Validation.png)