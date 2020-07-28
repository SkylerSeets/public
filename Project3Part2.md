![4827.jpeg](https://raw.githubusercontent.com/ashuang2013/public/master/4827.jpeg) <br/>
![6212.jpeg](https://raw.githubusercontent.com/ashuang2013/public/master/6212.jpeg) <br/>
![8197.jpeg](https://raw.githubusercontent.com/ashuang2013/public/master/8197.jpeg) <br/>

These are three images that I pulled from the complete 10000 image dataset. I made sure to only choose images that were not seen by the model in the training set (images inside the training set between 251.jpeg and 9000.jpeg) since I only trained the model on the first 250 images. <br/>

The model returned 0.04274386 for 4827.jpeg compared to the real value 68.8593444824219. <br/>
The model returned 0.04743501 for 6212.jpeg compared to the real value 46.7590255737305. <br/>
The model returned 0.04669612 for 8197.jpeg compared to the real value 110.827850341797. <br/> 

I believe that the model was trained on too little data, as I can only manage about 250 images. This is what I believe is giving my model such bad predictions.
