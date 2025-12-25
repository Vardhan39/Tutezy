# Tutezy
Tutezy is a modern EdTech platform that connects students with verified tutors for online and home tuition. Built using React, Firebase Authentication, and Firestore, it supports role-based access (Student/Tutor), secure authentication, tutor discovery, and a clean, scalable architecture designed for real-world education needs.
📱 Tutezy – Android EdTech Application

Tutezy is a modern Android-based EdTech application that connects students with verified tutors for online and home tuition. The app uses Firebase Authentication and Cloud Firestore to provide secure login, role-based access (Student/Tutor), and scalable data management.

🚀 Features

Firebase Email/Password Authentication

Role-based access (Student / Tutor)

Student & Tutor dashboards

Tutor discovery (future-ready)

Clean, modern UI inspired by top apps

Shared backend with Tutezy Web platform

🛠 Tech Stack

Language: Java

IDE: Android Studio

UI: XML (ConstraintLayout)

Architecture: MVVM (recommended)

Backend: Firebase Authentication & Firestore

📂 Project Structure
com.tutezy.app
│
├── ui
│   ├── auth
│   │   ├── SplashActivity.java
│   │   ├── LoginActivity.java
│   │   ├── SignupActivity.java
│   │
│   ├── student
│   │   ├── StudentDashboardActivity.java
│   │   ├── SearchTutorActivity.java
│   │
│   ├── tutor
│   │   ├── TutorDashboardActivity.java
│   │   ├── TutorProfileActivity.java
│
├── model
├── repository
├── viewmodel
├── utils
└── MainApplication.java

🔐 Firebase Configuration (Required)
1️⃣ Create Firebase Project

Go to Firebase Console

Create a new project named Tutezy

2️⃣ Enable Services

Authentication → Email/Password

Firestore Database → Test Mode

3️⃣ Add Android App

Package name: com.tutezy.app

Download google-services.json

⚙️ Project Setup in Android Studio
Step 1: Clone Repository
git clone https://github.com/your-username/tutezy-android.git

Step 2: Open in Android Studio

Open Android Studio

Select Open an existing project

Choose the cloned folder

Step 3: Add Firebase Config File

Place the downloaded file here:

app/google-services.json


⚠️ Do NOT rename the file
⚠️ Do NOT place it inside res or src

Step 4: Sync Project

Click Sync Project with Gradle Files

Ensure build completes successfully

▶️ Running the Application

Connect a physical Android device
OR

Start an Android Emulator

Then click:

Run ▶️

🔑 Authentication Flow

Users sign up using Email & Password

Select role: Student or Tutor

User data stored in Firestore (users collection)

Login redirects based on role:

Student → Student Dashboard

Tutor → Tutor Dashboard

🗄 Firestore Data Model

Collection: users
Document ID: Firebase UID

{
  "uid": "string",
  "name": "string",
  "email": "string",
  "role": "Student | Tutor",
  "createdAt": "timestamp"
}

🛡 Security Notes

Firebase handles secure authentication

Firestore rules restrict users to their own data

No credentials are hardcoded in the app

🎯 Use Cases

Hackathon submission

Academic mini / major project

Startup MVP

Scalable EdTech solution

📄 License

MIT License

✨ Author

Tutezy – Built for accessible, trusted, and personalized education.
