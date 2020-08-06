*__Problem Statement__*: <br/>
Unless you have been living under a rock or believe in conspiracy theories, it has been almost 5 months since the coronavirus was declared a pandemic by the WHO. The impacts on our daily lives have been...unexpected. As such, I hope to apply what I have learned this summer in both DATA 146 and 310 to create a model that will take certain features and output its contribution towards survival. I hope that this model can be analyzed and increase everyone's ability to survive should they catch the coronavirus since they will know which features are more important and prioritize them. <br/> 

*__Additional Descriptions__*: <br/>
I will be repurposing the Titanic model where we analyzed whether an individual would die based on many features. I will gather wholistic [data](https://ashuang2013.github.io/public/FinalProjectData) on the current coronavirus pandemic and apply it to a boosted tree and linear estimator model and compare their accuracies. The largest part will be preprocessing the data so that it can be read by the model. Another potential problem will be understanding the output through graphs. As of August 3rd, there are 4,694,126 people that tested positive and 147,653 people who have died to coronavirus or coronavirus-related complications. This virus has touched everyone, whether its a immediate or close family member, a friend, or a mentor. <br/> 
The Titanic model takes in multiple features and determines which features are important to an individual's survival as a percentage. This model takes in data and encodes it inside feature columns which are then used to create input functions for the model. The input functions are then inputted into both a boosted tree and linear estimator model where their accuracies will be compared. I then plan to create a violin plot in order to assess the model's results. The violin plot will allow me to see which features had a large or small effect on coronavirus survival on a broad scale. <br/>
I do not anticipate this to be a very complicated process, I am simply using some already written code and repurposing it with new data (at least I hope). The reason I believe that preprocessing the data will be a large problem is because each dataset is unique. Not only that, but every model is very specific in its inputs. I have to understand what the model wants and figure out a way to preprocess my data to match the model input specifications. 

For a larger timeline on the coronavirus, check out this website by the New York Times: <br/>
https://www.nytimes.com/article/coronavirus-timeline.html

Source: <br/>
https://www.tensorflow.org/tutorials/estimator/boosted_trees <br/>
https://www.tensorflow.org/tutorials/estimator/boosted_trees_model_understanding
