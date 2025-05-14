# 💪 Passion Fitness

**Passion Fitness** is a modern Android wellness and productivity app designed to help users track and improve their daily health habits. With an intuitive interface and a range of integrated features, it supports users in maintaining physical and mental well-being — all while keeping personal data secure and organized.

---

## 📱 Core Features

### 🔢 BMI Calculator
- Manually input height and weight.
- Calculates Body Mass Index (BMI).
- Results can be saved to the **Progress Diary**.

### 👣 Step Counter
- Uses the device's built-in step sensor to track daily steps.
- Step data is persistent and saved locally.
- Tied to each user's profile via UID.
- Shared Preferences maintains step states per user, even after logout.
- Daily step count can be saved to the **Progress Diary**.

### 🍎 Calorie Tracker
- Scan food barcodes using the camera to fetch product names and calorie info.
- Open Food Facts API integration.
- Manual calorie input also available.
- Save entries to the **Progress Diary**.

### 🌙 Sleep Tracker
- Input sleep duration and number of wake-ups.
- REM sleep estimated by deducting 0.5 hours per wake-up.
- Save data to the **Progress Diary**.

### 📔 My Diary
- Displays logged data from BMI, Steps, Calories, and Sleep.
- Helps users track trends and progress across all activities, including daily step counts.

### 💬 Inspire Me
- Displays a random inspirational quote via the ZenQuotes API.
- Encourages motivation and a positive mindset.

---

## 🔐 Authentication

- Full login and registration with **Firebase Authentication**.
- User-specific data storage using Firebase UID.

---

## 📦 Local Data Storage

- Offline support via **Room** database.
- Data tied to each Firebase UID.
- **SharedPreferences** stores step count state per user, even after logout.

---

## 🧭 Navigation Structure

- **Login Screen**: Sign in or navigate to registration.
- **Register Screen**: Create a new account.
- **Home Screen**: Access all key features.
- **Bottom Toolbar Navigation**:
  - Home
  - Profile
  - Logout
- **User Profile**:
  - View and manage account
  - Navigate home or logout
  - Option to delete account

---

## 📷 Camera Integration

- CameraX and ML Kit Barcode Scanning used in Calorie Tracker.
- Allows food scanning for nutritional data retrieval.

---

## 🛠️ Tech Stack

- **Language**: Kotlin  
- **UI**: Jetpack Compose  
- **Navigation**: Jetpack Navigation Component  
- **Authentication**: Firebase Auth  
- **Local Storage**: Room + SharedPreferences  
- **Camera & ML**: CameraX + ML Kit  
- **Concurrency**: Kotlin Coroutines  
- **APIs**:
  - [Open Food Facts API](https://wiki.openfoodfacts.org/API/Android)
  - [ZenQuotes API](https://zenquotes.io/)

---

## ✅ Best Practices Followed

- MVVM architecture (Model-View-ViewModel)
- Single Responsibility Principle (SRP)
- ViewModels manage UI state and lifecycle
- Repository pattern separates data concerns
- Modular, testable components

---

## 🚀 Presentation Link  
[Watch the presentation on YouTube](https://youtu.be/16fvQow0sS0)

