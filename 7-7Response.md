# QUESTION 1
'''
According to Maroney, Machine Learning is using the computer to create the rules that governs a program using both input and output data. The difference
between traditional programming and machine learning is the orientation of the process of writing code. For traditional programming, the programmer looks
at the input and output and formulates rules that govern them and the write the code. For machine learning, instead of the programmer writing the rules, 
the machine will look at both the input and the output and find the rules that govern them.
'''

# QUESTION 2
# The first prediction is 21.996738
# The second prediction is 21.999975
'''
The difference between the two depends on where the computer guesses and how accurate its first guess is. Depending on how close the computer guesses, the subsequent
reduction through MSE will reduce causing a slight difference in the final prediction.
'''

# QUESTION 3
'''
The home that costs $97,000 with 3 bd and 1 ba is the best deal since it has the greatest difference from the predicted price using the model that was fit to the 6 homes.
The home that costs $577,200 with 5 bd and 2 ba is the worst deal since it has the greatest difference from the predicted price using the model.

I fit a model on the given home prices and then compared each home's bedroom to the original given model of 50 + 50x where x is the number of bedrooms. Then the model predicted the price for each bedroom. Then this predicted price was subtracted from the original given model with the same number of bedrooms. The result with the highest and lowest price are the worst and best houses respectively. 
'''
