

---

## 🥗 FoodCalci - Your Personal Food Tracker

**FoodCalci** is a lightweight web app that uses **AI image recognition** to detect foods from uploaded images and estimate their **calorie values** by integrating with the **USDA FoodData Central API**.

Try out **FoodCalci** live:

👉 [https://staging.d282j2d0ipgah1.amplifyapp.com/](https://staging.d282j2d0ipgah1.amplifyapp.com/)

> Upload a photo of your food — get instant calorie estimates in your browser.

---

### 🚀 Features

* 📷 Upload any food image
* 🧠 Detects food items using **AWS Rekognition**
* 🔍 Estimates real calories using **USDA FoodData Central API**
* 📊 Shows top detected food labels with confidence scores
* 💾 Remembers last uploaded result with **localStorage**
* 🎨 Clean UI, fully responsive
* ♿ Keyboard accessible & ARIA-friendly

---

### 📦 Tech Stack

| Feature         | Tech Used                         |
| --------------- | --------------------------------- |
| Image Detection | AWS Rekognition (via browser SDK) |
| Calories API    | USDA FoodData Central API         |
| Auth            | AWS Cognito Identity (anonymous)  |
| UI              | HTML, CSS, JavaScript             |
| Storage         | `localStorage`                    |

---

### 🖼️ Demo

> Upload an image (e.g., of a banana, burger, salad) and view calories instantly.
> Example output:

```
Name of food     Confidence
Banana           100.00
Fruit            100.00
Food             100.00
------------------------------
Estimated Calories: 89 Kcal
```

---

### 🛠️ Setup Instructions

1. Clone or download this repository
2. Place your own background image as `background.jpg` in the same directory
3. Open `index.html` in your browser or use amplify to host on AWS.

> **Note**: You must have internet access to load AWS + USDA APIs from CDN.

---

### 🔐 API Keys Required

1. **USDA API Key**
   Sign up at [https://api.data.gov/signup](https://api.data.gov/signup) and get a free API key.
   Replace the placeholder in `index.html`:

   ```js
   const apiKey = 'YOUR_API_KEY_HERE';
   ```

2. **AWS Cognito Identity Pool ID**
   Used for anonymous Rekognition access.
   Replace this with your own identity pool:

   ```js
   IdentityPoolId: 'Replace with your pool ID'
   ```

---

### ⚠️ Limitations

* Calorie values are typically per 100g (as provided by USDA).
* Rekognition may return non-food labels
* No server backend — everything runs client-side (keys are visible in browser).
* USDA database may not return exact matches for all labels.

---

### 📈 Future Improvements

* Filter non-food labels automatically
* Add portion-size selector (e.g., 1 apple, 1 slice, etc.)
* Use a backend to hide API keys and cache frequent foods
* Add nutrition breakdown (protein, carbs, fats)

---

### 📄 License

This project is open-source and MIT licensed.

---