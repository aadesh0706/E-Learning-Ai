![Profile Views](https://komarev.com/ghpvc/?username=aadesh0706&color=blue)  
*Active since*: `September 2024`

# 🚀 E-Learning AI Platform

Welcome to the **E-Learning AI Platform**! This platform allows users to sign up, log in, and track their progress using Firebase Authentication. The project is built using **React** and hosted with **Firebase Hosting**.

> **Current Features:**
> - 👨‍🎓 User authentication (Login & Signup) using Firebase Auth.
> - 📊 Dashboard that adds 10 points to the user's score with every button click and stores it in the Firestore.
> - 🔐 Protected routes that ensure only logged-in users can access the dashboard.

---

## 🖥️ Demo
🌐 [Live Site](https://e-learning-ai.web.app)

---

## 📜 Table of Contents
- [Demo](#demo)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Technologies Used](#technologies-used)
- [Contributing](#contributing)
- [License](#license)

---

## ✨ Features

- **User Registration**: New users can sign up using email and password.
- **Login & Logout**: Users can log in and log out securely.
- **Protected Routes**: Only authenticated users can access the Dashboard.
- **Score Tracking**: Users can click a button on the dashboard to increase their score, which is stored in Firebase Firestore.
- **Firebase Hosting**: Deployed with Firebase Hosting for fast and secure hosting.

---

## 🛠️ Installation

Follow the steps below to get this project up and running locally.

### Prerequisites

- 📦 Node.js v14 or above installed
- Firebase CLI installed globally: `npm install -g firebase-tools`
- A Firebase project with Authentication and Firestore enabled

### Clone the Repository

```bash
git clone https://github.com/your-username/e-learning-ai.git
cd e-learning-ai
```

### Install Dependencies

```bash
npm install
```

### Firebase Setup

1. **Configure Firebase**: Create a Firebase project in the Firebase Console.
2. **Add Firebase SDK**: Add the Firebase configuration to your `firebase.js` file.

```javascript
// firebase.js
import { initializeApp } from "firebase/app";
import { getAuth } from "firebase/auth";
import { getFirestore } from "firebase/firestore";

const firebaseConfig = {
  apiKey: "YOUR_API_KEY",
  authDomain: "YOUR_AUTH_DOMAIN",
  projectId: "YOUR_PROJECT_ID",
  storageBucket: "YOUR_STORAGE_BUCKET",
  messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
  appId: "YOUR_APP_ID"
};

const app = initializeApp(firebaseConfig);
export const auth = getAuth(app);
export const db = getFirestore(app);
```

### Run Locally

```bash
npm start
```

The app will be live at `http://localhost:3000`.

---

## 🚀 Deployment

To deploy your app on Firebase Hosting, follow these steps:

1. **Build the app**:

```bash
npm run build
```

2. **Deploy to Firebase**:

```bash
firebase login
firebase init
firebase deploy
```

Your app will be deployed to Firebase Hosting!

---

## 📂 Project Structure

Here's an overview of the project structure:

```bash
📦 e-learning-ai
├── 📁 public         # Public assets
├── 📁 src            # Source code
│   ├── 📁 components # React components (Login, Signup, Dashboard)
│   ├── App.js        # Main React component
│   ├── firebase.js   # Firebase configuration
│   └── index.js      # Entry point
├── .firebaserc       # Firebase project settings
├── firebase.json     # Firebase Hosting configuration
└── package.json      # Project dependencies
```

---

## 🛠️ Technologies Used

- **React**: Frontend framework for building UI.
- **Firebase**: Backend services for authentication, database, and hosting.
  - **Firebase Authentication**: Secure user login and signup.
  - **Firebase Firestore**: Store user data and scores.
  - **Firebase Hosting**: Host the application.

---

## 🤝 Contributing

We welcome contributions to make this platform even better!

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeature`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature/YourFeature`).
5. Open a pull request.

---

Made with 💙 by [Your Name](https://your-profile-link) 🌟

---

Feel free to replace the **Firebase config**, **repo URL**, **username**, and **live demo link** with your actual project details before using this README.

This structure should help users quickly understand the project, install it, and contribute. If you need further customization, let me know! 😊
