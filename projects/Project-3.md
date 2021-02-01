---
layout: project
type: project
image: images/MLProj2.jpg
title: Skin Disease Detection Web App
permalink: 
# All dates must be YYYY-MM-DD format!
date: 2021-01-05
labels:
  - Python
  - Flask
  - TensorFlow
  - Heroku
summary: I built a Machine Learning web app in Flask for my friend who wanted to deploy their Machine Learning model online.
---

<div>
  <img src="../images/Sys Arc 11.22.png">
  <img src="../images/opnn sys 11.21.png">
</div>


Description
No Machine Learning model is truly complete without a interface that lets regular people interact with the model.
A UI is even more important for models that deal with image processing, as testing it against real world picture would put it to the real test.
My friend, who is studying in the field of Machine Learning, came to me to help him deploy his Machine Learning model on the web. 
It was an interesting case as I had to figure out how to connect his model with Flask and then represent the result on the front end.

Technical Details
I had to implement multiple Flask functions to have form submission, in our case only image would suffice and that was handled with WTForms. 
After the image submission was successful, the picture was to be stored in the local directory. A ML function would then take the image from the directory
and run the model on that. Finally, the prediction would be returned and grabbed a final function that would display the results on the front page. 
The final function would also redirect the user to the results page on submission as I believed that was the right UI design to implement because this 
would protect the app from multiple uploads on one session which is not something that can be handled by the app. 

I also had a diffcult time trying to deploy this app on Heroku as they did not like the tensorflow package size and therefore slowed 
down our app for initial boot.

Conclusion
This was my first attempt at Flask web app. I can definitely implement better process handling, such as implementing Celery from python. 
Also need to find a better platform for deploying ML Web Apps as the slug size of heroku limits deployement of Image Processing Models.

