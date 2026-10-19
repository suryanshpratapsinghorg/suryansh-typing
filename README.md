# SURYANSH TYPING — Touch Typing Learning Website

**SURYANSH TYPING** is a browser-based touch-typing tutor designed to help beginners learn to type without constantly looking at the keyboard. It combines progressive typing lessons with a dark hacker-style interface, live feedback, and simple progress tracking.

> **Goal:** Build typing accuracy first, then gradually improve speed and confidence.

## ✨ Features

- **100 Learning Lessons** — practice from home-row keys to words, sentences, punctuation, numbers, symbols, and basic code snippets.
- **Live typing feedback** — highlights the current character and marks typed characters as correct or incorrect.
- **Typing statistics** — view words per minute (WPM), accuracy, errors, and remaining time during lessons.
- **Lesson completion results** — receive a star rating and choose to retry or continue to the next lesson.
- **Practice mode** — type sample passages at your own pace.
- **Typing race** — move your racer forward as you type the passage.
- **Virtual keyboard** — highlights the next key to press.
- **Different test durations** — choose 30 seconds, 60 seconds, or 2 minutes.
- **Progress dashboard** — view your best WPM, completed lessons, average accuracy, and typed characters.
- **Hacker-inspired visual design** — dark interface with a Matrix-style animated background.
- **Optional Firebase authentication** — supports email/password accounts and Google sign-in after the owner configures Firebase.
- **Responsive layout** — designed for use in a modern desktop or mobile browser.

## 🧰 Built With

- HTML5
- CSS3
- Vanilla JavaScript (ES modules)
- Firebase Authentication (optional; requires configuration)
- Browser `localStorage` for local typing statistics

## 📁 Project Structure

```text
SURYANSH_TYPING_Learning_Lessons_Login_Source/
├── index.html            # Main website structure
├── css/
│   └── style.css         # Styling, layout, and responsive design
├── js/
│   ├── app.js            # Lessons, typing logic, race, and progress
│   └── firebase-auth.js  # Optional Firebase sign-in/sign-up
├── assets/               # Place images or other static assets here
└── README.md             # Project documentation
```

## 🚀 Run the Website Locally

1. Download or clone this repository.
2. Keep the folder structure unchanged.
3. Open the project folder in Visual Studio Code.
4. Start the site with a local development server, such as the **Live Server** extension.
5. Open the local URL provided by the server and select a lesson to begin typing.

You can also open `index.html` directly for the basic typing interface. For best compatibility—especially with the Firebase ES module—use a local server.

## 🔐 Set Up Firebase Authentication (Optional)

Sign-in and account creation will not work until Firebase is configured. The typing lessons can be used without setting up authentication.

1. Create a project in the [Firebase Console](https://console.firebase.google.com/).
2. Add a Web App to the Firebase project and copy its web configuration.
3. In `js/firebase-auth.js`, replace the placeholder values in `firebaseConfig` with your project's values:

   ```js
   const firebaseConfig = {
     apiKey: 'YOUR_FIREBASE_API_KEY',
     authDomain: 'YOUR_PROJECT_ID.firebaseapp.com',
     projectId: 'YOUR_PROJECT_ID',
     appId: 'YOUR_FIREBASE_APP_ID'
   };
   ```

4. In Firebase Console, open **Authentication → Sign-in method** and enable **Email/Password** and **Google** providers as needed.
5. Add your local development domain and deployed website domain to Firebase's authorized domains if required.
6. Run the site through a local server and test sign-in/sign-up.

**Security note:** Never put a Google account password into this website. Use the Google sign-in button for Google accounts. Firebase web configuration is intended for client-side use, but protect your project with appropriate Firebase security rules and settings. Do not commit private service-account keys or other server secrets to GitHub.

## 📊 How Progress Is Stored

Typing statistics are stored in the current browser using `localStorage`. This means progress is generally limited to that browser and device; it is **not automatically synced to a cloud database or across devices**. Clearing browser site data can remove locally saved progress.

## 🎯 Tips for Learning Touch Typing

1. Keep your fingers near the home row: **A S D F** and **J K L ;**.
2. Look at the screen rather than your keyboard when possible.
3. Aim for accuracy before trying to type quickly.
4. Practise for a short time every day instead of rushing through many lessons at once.
5. Keep your shoulders relaxed and take breaks when needed.

## 🌐 Creator & Links

- **Project:** SURYANSH TYPING
- **Instagram:** [@suryanshpratapsinghofficial](https://www.instagram.com/suryanshpratapsinghofficial/)
- **Website:** [Suryansh Official](https://suryanshpratapsingh.wixsite.com/suryansh)

## 📄 License

No license has been specified for this project yet. If you want others to reuse, modify, or distribute the source code, add a suitable open-source license file (for example, an MIT License) before publishing.

---

© 2026 SURYANSH TYPING. All rights reserved.
