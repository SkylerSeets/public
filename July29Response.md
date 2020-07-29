# QUESTION A
Sources: <br/>
a. https://www.cnn.com/2020/07/29/politics/stella-immanuel-trump-doctor/index.html <br/>
b. https://www.washingtonpost.com/national/at-the-heart-of-dismal-us-coronavirus-response-a-fraught-relationship-with-masks/2020/07/28/f47eccd0-cde4-11ea-bc6a-6841b28d9093_story.html <br/>
c. https://www.foxnews.com/us/minnesota-coronavirus-mask-mandate-nazi-star-david <br/>
d. https://www.npr.org/2020/07/29/896649636/tiktok-ceo-facebook-is-making-copycat-service-disguised-as-patriotism <br/>
e. https://www.cnn.com/2020/07/29/health/us-coronavirus-wednesday/index.html <br/>

The model gives the above 5 articles these scores respectively (0.98858625, 0.98763394, 0.00141422, 0.00814823, 0.08367229). The model predicted that articles a and b were sarcastic and articles c, d and e were not sarcastic. I partially chose the articles a and b partially because they sounded too impossible to be true. <br/> 
Article a, which promotes a scientist that is using *alien* DNA to cure coronavirus. This headline is hard to believe, and thus not surprising that it was classified as sarcasm by the model. <br/>
Article b, which once again held a grain of truth in our *"interesting"* world we find ourselves in right now. I was actually very interested to see how the model would classify this article. I was surprised to see the model classify this as sarcasm. Unlike the previous article, which had very obvious trigger words like alien, this article did not. I'm guessing that the model itself classified masks and coronavirus response together as not sarcastic, and the disparate words fraught (which indicates undesireability), being combined with a positive situation created a duality that resulted in the model saying the article was sarcastic. <br/>
Articles c, d and e are standard articles that I chose just to make sure that the model was predicting properly. They are the standard headlines which give a general overview of the contents in the article. 

# QUESTION B
An RNN differs from other models in that it has an "internal state that depends on previously seen elements." This means that the RNN model remembers all its characters outputted, and based on the outputs, it computes the next output. This ability to remember outputs is what allows the model to basically "learn" and then "reproduce" Shakspeare. The model seems to do very well on the overall text structure, but struggles in making coherent and grammarly correct sentences. <br/>
Source: https://www.tensorflow.org/tutorials/text/text_generation

# QUESTION C
I believe that the model did a pretty good job with the translations 2.9/3. I don't agree with the translation by the model hace much frio aqui to its nice cold here. I'm rusty on my Spanish but I believe that this should be translated to its very cold here.
