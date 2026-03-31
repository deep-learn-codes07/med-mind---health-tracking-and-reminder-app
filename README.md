# med-mind---health-tracking-and-reminder-app

# MedMind 💊

MedMind is a comprehensive health management Android application designed to help users track their medications, monitor vital health statistics, and integrate data from wearable devices.

## 🚀 Features

- **Medication Tracking**: Log and manage daily medicine schedules.
- **Smart Health Monitoring**: 
    - **Step Counter**: Live tracking of steps using device sensors.
    - **Water Intake**: Monitor daily hydration levels.
    - **BPM Tracking**: Log and visualize heart rate data.
- **Smart Watch Integration**: Sync health data (Steps, Heart Rate) from wearables using Google Play Services and Health Connect.
- **AI & ML Capabilities**:
    - **OCR (Optical Character Recognition)**: Scan medicine labels using ML Kit Text Recognition.
    - **Barcode Scanning**: Quickly identify products via Barcode Scanning.
    - **Generative AI**: Integration for smart health insights.
- **Firebase Integration**: Real-time database for user data and secure Authentication.
- **Payments**: Integrated Razorpay for health-related store purchases.

## 🛠 Tech Stack

- **Language**: Java / Kotlin (DSL for Gradle)
- **Database**: Firebase Realtime Database
- **Authentication**: Firebase Auth & Google Sign-In
- **AI/ML**: Google ML Kit (Text & Barcode), Google Generative AI
- **Health**: Health Connect, Google Fit API, Wearable Support
- **Networking**: Retrofit 2, OkHttp 3
- **UI Libraries**: 
    - `MPAndroidChart` (Data Visualization)
    - `CircleProgress` (Health Goals)
    - `Glide` (Image Loading)

## 📋 Prerequisites

- Android Studio Ladybug or newer.
- Android SDK 31 (Android 12) or higher.
- A Firebase Project (with `google-services.json` placed in the `app/` directory).

## ⚙️ Installation & Setup

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/medmind.git
   ```

2. **Firebase Configuration**:
   - Go to the [Firebase Console](https://console.firebase.google.com/).
   - Add a new Android Project with the package name `com.example.medmind`.
   - Download the `google-services.json` and place it in the `app/` folder.
   - Enable **Authentication** (Google & Email) and **Realtime Database**.

3. **Build the Project**:
   - Open the project in Android Studio.
   - Clean the project: `Build > Clean Project`.
   - Sync Gradle files.

4. **Permissions**:
   The app requires the following permissions for full functionality:
   - `ACTIVITY_RECOGNITION` (for Live Steps)
   - `CAMERA` (for ML Kit Scanning)
   - `BODY_SENSORS` (for Heart Rate)

## 🏗 Project Structure

- `HealthStepsActivity.java`: Manages live step counting and UI progress.
- `HealthConnect.java`: Logic for syncing data from smartwatches and Google Fit.
- `utils/`: Contains `FirebaseHelper` and `HealthDataManager` for data persistence.
- `libs.versions.toml`: Centralized dependency management using Version Catalogs.

## 🤝 Contributing

1. Fork the Project.
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`).
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`).
4. Push to the Branch (`git push origin feature/AmazingFeature`).
5. Open a Pull Request.

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.

---
*Developed as part of the MedMind Health Solution.*
