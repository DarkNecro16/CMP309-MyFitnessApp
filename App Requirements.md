# ✅ Requirements Fulfilment: Passion Fitness App

This document outlines how the **Passion Fitness** application satisfies the requirements of Task 1 CMP309 - Mobile Software Development 
---

## 📌 Native Android App in Kotlin

- Developed entirely in **Kotlin** using **Native Android APIs**.
- Compatible with devices/emulators running **API Level 33+**.
- Built with **Android Studio** and Jetpack libraries.

---

## 🧱 Object-Oriented Programming & Architecture

- The app adheres to **Object-Oriented Programming (OOP)** principles:
  - Clear separation of concerns through structured packages: `AppLogic`, `Database`, `ViewModel`, and `UI`.
  - Code is organized using **classes**, **inheritance**, and **encapsulation** to promote maintainability and reusability.

- Follows the **Model-View-ViewModel (MVVM)** architecture:
  - **UI layer** (Activities/Compose) handles user interaction and rendering.
  - **ViewModel layer** manages UI-related logic and lifecycle-aware data (e.g. LiveData, State).
  - **AppLogic layer** contains business logic (e.g. barcode scanning, calculations).
  - **Database layer** handles local data persistence using Room and SharedPreferences.
  - Encourages scalability and testability through clear separation between data, logic, and presentation.

---

## 🔄 Component Communication

- Uses multiple Android **application components**:
  - **Activities**: LoginActivity, RegisterActivity, HomeActivity, ProfileActivity, etc.
  - **ViewModels**: Maintain state and logic per feature (e.g., CalorieTrackerViewModel).
- Clear communication between components:
  - Navigation via **Intents** between Activities.
  - SharedPreferences and Room handle data flow.
  - ViewModel communicates with Repository.

---

## 📱 User Interface & Screens

- Contains **more than 3 functional and interactive screens**:
  1. **Login/Register**
  2. **Home Dashboard** (Central Hub of App)
  3. **BMI Calculator**
  4. **Step Counter**
  5. **Calorie Tracker**
  6. **Sleep Tracker**
  7. **Progress Diary**
  8. **Inspire Me**
  9. **Profile Management**

- UI built using **Jetpack Compose**

---

## 🔁 Lifecycle & Input Handling

- Lifecycle managed with **ViewModels**, **LiveData**, and **State** in Compose.
- Proper handling of orientation changes and configuration shifts.
- Persistent data using **Room** and **SharedPreferences** ensures input/state retention across sessions and logins.

---

## 💾 Data Storage & 🌐 Connectivity

### Storage:
- **Room Database**: Stores user-specific data (BMI, steps, sleep, calories).
- **SharedPreferences**: Maintains step count state tied to individual UIDs.
- Data tied to Firebase UIDs to maintain isolation between users.

### Connectivity:
- **Camera + ML Kit Barcode API**: For scanning food items.
- **Open Food Facts API**: Retrieves food details via HTTP.
- **ZenQuotes API**: Fetches motivational quotes.
- **Firebase Authentication**: Handles login, register, and account deletion via cloud.

---

## 🔒 Usability, Security & Performance

- **Authentication**: Firebase secures user accounts and database access.
- **User Isolation**: Data is scoped to UID to ensure privacy.
- **Efficient Threading**: All network/database operations are run with **Kotlin Coroutines** on background threads.
- **Permissions**: Runtime permissions requested for camera and network access.
- **Data Handling**: Input validation, error messages, and try-catch blocks used throughout.
- **Battery/Resource Friendly**: Efficient sensor use and unregistered listeners when not in use.

---

## ♿ Accessibility & UX Considerations

- Clean, simple UI designed for clarity and readability.
- Touch-friendly layouts and feedback on user actions.
- Future consideration for:
  - Dark mode
  - Larger text options
  - Voice Assistant integrations

---

## 🎯 Summary of Key Features Implemented

| Requirement                                 | Implemented in App                            |
|--------------------------------------------|-----------------------------------------------|
| Kotlin / Native APIs                       | ✅ Yes                                          |
| Minimum 2 Components with Communication    | ✅ Activities, ViewModels, SharedPreferences   |
| 3+ Interactive Screens                     | ✅ 9+ Activities/Screens                        |
| Lifecycle & Input Handling                 | ✅ ViewModel, LiveData, SharedPreferences      |
| Data Storage Feature                       | ✅ Room + SharedPreferences                    |
| Connectivity Feature                       | ✅ Barcode API, Open Food Facts, Firebase      |
| Usability, Security, and Performance       | ✅ Authentication, Coroutines, Permissions     |
| Optional Accessibility                     | ⚠️ Basic structure present, room for expansion|

---

> ✅ This document provides clear evidence that the Passion Fitness app successfully meets and exceeds the Task 1 development requirements as outlined in the assignment brief.
