# FoodCalci - Your Personal Food Tracker

FoodCalci is a proof-of-concept web application compatible across all devices (PC, smartphones). It allows users to upload local images of food, then uses **AWS Rekognition** to classify the image and estimate the calorie content.

The app is deployed on AWS and ready to use.

---

## Live Demo

Try the web app on any device here:  
[https://dev.d32zqi8gqqbshs.amplifyapp.com](https://dev.d32zqi8gqqbshs.amplifyapp.com)

---

## How to Use

1. Upload an image from your device or use sample images provided in the `sample-images` folder.
2. The app sends the image to AWS Rekognition for classification.
3. Within seconds, the app displays:
   - Image classification results with confidence score (0-100)
   - Approximate calorie estimation based on classification

---

## Getting Started

To run or customize this web app:

```bash
git clone https://github.com/dineshuday/FoodCalci-WebApp-for-calorie-calculation-using-AWS-rekognition.git
````

Feel free to modify and extend the app for other AWS Rekognition use cases like:

* Celebrity identification
* PPE kit detection
* Exam proctoring

---

## Technologies Used

* AWS Rekognition (Image classification)
* AWS Amplify (Hosting)
* JavaScript (frontend)

---

If you have any questions or want to contribute, please open an issue or a pull request.

---
