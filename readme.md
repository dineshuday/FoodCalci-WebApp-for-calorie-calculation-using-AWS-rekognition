FoodCalci - Your personal food tracker

This project is proof of concept web application that is compatible in all devices, used to upload local images stored in a pc or smartphone, and once uplaoded its hits the aws rekognition service for image classification and then calorie calculation.
The web app is already deployed on to the aws cloud.

To Run and test the webapp proof of concept
- Visit this URL in any device : https://dev.d32zqi8gqqbshs.amplifyapp.com
- Upload the image from the sample-images folder or any local images from your device.
- Once uploaded within few seconds, it will hit the aws rekognition service and then returns the response of image classification along with the confidence range from 0-100 and also the approximate calorie value.

- use git clone to clone this repo and make modiciations to play around this webapp and use this for other rekognition service like celebrity identificaiton, PPE kit identification, and exam proctoring etc.