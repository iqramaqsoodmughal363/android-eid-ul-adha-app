# 🌙 Eid ul Adha Companion App

<p align="center">
  <b>Celebrate the spirit of sacrifice with a complete Eid ul Adha experience.</b>
</p>

<p align="center">
  <em>"A comprehensive Android application built in Java featuring Qurbani guides, Takbeer audio, Kids Corner, Quizzes, and animated Fireworks."</em>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Made%20with-%E2%9D%A4%EF%B8%8F-red" alt="Made with Love">
  <img src="https://img.shields.io/badge/Platform-Android-green" alt="Platform">
  <img src="https://img.shields.io/badge/Language-Java-orange" alt="Language">
  <img src="https://img.shields.io/badge/Theme-Eid%20ul%20Adha-blueviolet" alt="Theme">
  <img src="https://img.shields.io/badge/Status-Complete-success" alt="Status">
</p>

---

## 📋 Overview

**Eid ul Adha Companion** is a beautifully designed Android application that enhances the festive experience of Eid ul Adha. Built entirely in **Java**, it combines educational, interactive, and entertainment features into one seamless app. From listening to Takbeer to playing quizzes and watching fireworks, this app has something for everyone in the family.

---

## ✨ Key Features

* **🐐 Qurbani Guide (`QurbaniActivity.java`):** Step-by-step guidance and information regarding the rules and practices of Qurbani.
* **🕌 Takbeer Audio (`TakbeerActivity.java`):** Listen to beautiful Takbeer recitations with play, pause, and stop controls.
* **🧒 Kids Corner (`KidsCornerActivity.java`):** A fun, interactive section designed specifically for children, featuring animal sounds (`dialog_animal_sound.xml`) and games.
* **🧠 Islamic Quiz (`ExtendedQuizActivity.java`):** Test your knowledge about Eid ul Adha and Islamic history with an interactive quiz (`dialog_quiz.xml`).
* **⏳ Countdown Timer (`CountdownActivity.java`):** A live countdown to the big day to build excitement.
* **🎆 Fireworks Animation (`FireworksActivity.java`):** A visually stunning fireworks display to celebrate the occasion.
* **📍 Nearby Places (`NearbyActivity.java`):** Find nearby mosques or Qurbani markets (requires location permission).
* **🔔 Notifications (`NotificationReceiver.java`):** Get timely reminders for Takbeer and prayer times.

---

## 🛠️ Tech Stack

| Category | Tools / Technologies |
|---|---|
| **Language** | Java |
| **IDE** | Android Studio |
| **UI Components** | XML Layouts, Custom Dialogs, Fragments |
| **Media Handling** | `MediaPlayer` (Takbeer Audio), `Animation` (Fireworks) |
| **Data Storage** | `SharedPreferences`, Local Assets (`raw` folder for audio) |
| **Notifications** | `BroadcastReceiver` (`NotificationReceiver.java`) |

---

## 📂 Project Structure

```text
android-eid-ul-adha-app/
│
├── app/
│   ├── src/
│   │   ├── main/
│   │   │   ├── assets/                          # Local HTML/JSON assets if any
│   │   │   ├── java/com/eiduladhaapp/
│   │   │   │   ├── CountdownActivity.java       # Timer for Eid
│   │   │   │   ├── ExtendedQuizActivity.java    # Islamic Quiz logic
│   │   │   │   ├── FireworksActivity.java       # Fireworks animation
│   │   │   │   ├── HomeActivity.java            # Main Dashboard
│   │   │   │   ├── KidsCornerActivity.java      # Kids games & sounds
│   │   │   │   ├── MainActivity.java            # Splash/Entry Activity
│   │   │   │   ├── NearbyActivity.java          # Location-based features
│   │   │   │   ├── NotificationReceiver.java    # Handles system notifications
│   │   │   │   ├── QurbaniActivity.java         # Qurbani rules & guide
│   │   │   │   └── TakbeerActivity.java         # Audio player for Takbeer
│   │   │   ├── res/
│   │   │   │   ├── drawable/                    # Icons (butcher, goat, play, stop, etc.)
│   │   │   │   ├── layout/                      # UI Layouts (activity & dialog XMLs)
│   │   │   │   ├── menu/                        # Options menu
│   │   │   │   ├── navigation/                  # Nav graph
│   │   │   │   ├── raw/                         # Takbeer audio files (.mp3)
│   │   │   │   ├── values/                      # Colors, Strings, Themes
│   │   │   │   └── xml/                         # Backup rules
│   │   │   └── AndroidManifest.xml
│   │   └── build.gradle.kts
│   ├── proguard-rules.pro
│   └── gradle/
├── build.gradle.kts
├── settings.gradle.kts
└── README.md
```

---

## 🚀 How to Build and Run

### Prerequisites
* **Android Studio** (Latest Version)
* **JDK 11** or higher
* **Android SDK** (API 21+)

### Steps

1. **Clone the Repository**
   ```bash
   git clone https://github.com/iqramaaqsoodmughal363/android-eid-ul-adha-app.git
   ```
2. **Open in Android Studio**
   Open Android Studio → **File** → **Open** → Select the project folder.
3. **Sync Gradle**
   Wait for Gradle to sync. Click **"Sync Now"** if prompted.
4. **Build and Run**
   Connect your Android device or start an emulator, then click the **Run** button (green play icon).

---

## ⚙️ How It Works (Behind the Scenes)

### 1. Multimedia & Audio (`TakbeerActivity.java` & `MediaPlayer`)
The Takbeer section uses Android's `MediaPlayer` class to load audio files from the `res/raw` folder. It provides a custom UI with Play, Pause, and Stop buttons for a smooth listening experience.

### 2. Interactive UI (`FireworksActivity.java` & `CountdownActivity.java`)
The app uses Android's `Animation` framework to create a lively fireworks display and a `CountDownTimer` class to count down the days, hours, and minutes until Eid.

### 3. Custom Dialogs (`dialog_quiz.xml` & `dialog_animal_sound.xml`)
Instead of full-screen activities for small tasks, the app uses custom `AlertDialogs`. For example, in Kids Corner, clicking an animal plays a sound via a popup dialog.

### 4. Background Notifications (`NotificationReceiver.java`)
The `NotificationReceiver` extends `BroadcastReceiver` to schedule and deliver important alerts (like prayer times or Takbeer reminders) even when the app is closed.

---

## 🎯 Key Takeaways

* **Event-Based App:** A perfect example of building an app for a specific festival/event.
* **Multimedia Integration:** Shows how to handle audio playback and complex animations in Android.
* **Family-Friendly:** Includes features for all age groups (Adults, Kids, Quiz lovers).
* **Java Fundamentals:** Solid demonstration of Java and Android UI lifecycle management.

---

## 👩‍💻 Author

**Iqra Maqsood Mughal**

*Software Engineer · Full-Stack Developer · Code Craftsman · Android App Developer · Problem Solver 🚀*

```javascript
const codeIsLife = "Code is life";
while (true) { 
    learn(); 
    build(); 
    innovate(); 
}
```

---

## 📅 Date

October 18, 2026

---

## 📄 License

This project is intended for educational and personal use purposes.
