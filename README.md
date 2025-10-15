# 🔥 Simple Firebase Database

A minimal and beginner-friendly Node.js project showing how to connect to **Firebase** and perform basic **CRUD (Create, Read, Update, Delete)** operations.  
Perfect for learning, experimenting, or bootstrapping small apps. 🚀

---

## 🧭 Table of Contents

- [✨ Features](#-features)
- [⚙️ Prerequisites](#️-prerequisites)
- [🧩 Installation](#-installation)
- [🔧 Configuration](#-configuration)
- [🧠 Usage](#-usage)
- [📂 Project Structure](#-project-structure)
- [🧾 Examples](#-examples)
- [🤝 Contributing](#-contributing)
- [📄 License](#-license)

---

## ✨ Features

✅ Connects to your Firebase project easily  
✅ Simple, readable code — ideal for beginners  
✅ Demonstrates CRUD operations step-by-step  
✅ Minimal dependencies and setup  
✅ Fully extendable to your own app  

---

## ⚙️ Prerequisites

Before starting, make sure you have:

- 🟢 Node.js (v12 or newer)
- 📦 npm or yarn
- 🔑 A Firebase project
- 📁 Firebase service account credentials (`.json`)

---

## 🧩 Installation

Clone the repository and install dependencies:

```bash
git clone https://github.com/Rranssu/Simple-Firebase-Database.git
cd Simple-Firebase-Database
npm install
```
---

##🔧 Configuration

You’ll need to set up your Firebase credentials inside server.js (or .env if you prefer environment variables).
```bash
const admin = require('firebase-admin');
const serviceAccount = require('./path/to/your-service-account.json');

admin.initializeApp({
  credential: admin.credential.cert(serviceAccount),
  databaseURL: "https://<YOUR_PROJECT_ID>.firebaseio.com"
});
```
---

##📝 Tips:

Replace the path/to/your-service-account.json with your actual credentials file.

Update databaseURL with your project’s Firebase URL.

For Firestore, use admin.firestore() instead of admin.database().
##🧠 Usage

Once you’re all set up, simply run:
```bash
node server.js
```
🎉 Boom! Your Firebase connection should be live — ready for reads, writes, and updates.\

---

##🤝 Contributing

Contributions are welcome! 🙌

Fork the repo

Create a new branch → git checkout -b feature/YourFeature

Commit your changes → git commit -m "Add feature XYZ"

Push your branch → git push origin feature/YourFeature

Open a pull request 🚀

---

##📄 License

This project is open-source and available under the MIT License
