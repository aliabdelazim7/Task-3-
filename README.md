# FlightTracker Android App

This is an Android application built with Android Studio and the Backpack UI library that displays flight information in a clean, card-based interface.

## Features

- **Flight Information Card**: Displays the flight number
- **Departure Card**: Shows departure airport code (LHR) and time (10:30 AM)
- **Arrival Card**: Shows arrival airport code (JFK) and time (1:45 PM)

## Prerequisites

- Android Studio (latest version, avoid Dolphin due to Backpack component bugs)
- Android SDK API 33 or higher
- Kotlin support

## Installation

1. **Install Android Studio**

   - Download from [developer.android.com/studio](https://developer.android.com/studio)
   - Follow the installation wizard
   - Note: Avoid Android Studio Dolphin due to Backpack component display issues

2. **Open the Project**

   - Open Android Studio
   - Select "Open an existing Android Studio project"
   - Navigate to this project folder and select it

3. **Sync Gradle**

   - When prompted, click "Sync Now" to download dependencies
   - The Backpack library (version 43.0.0) will be automatically downloaded

4. **Run the App**
   - Click the green "Run" button (▶️) in the toolbar
   - Select your emulator or connected device
   - The app will build and launch

## Project Structure

```
app/
├── src/main/
│   ├── java/com/example/flighttracker/
│   │   └── MainActivity.kt
│   ├── res/
│   │   ├── layout/
│   │   │   └── activity_main.xml
│   │   ├── values/
│   │   │   ├── strings.xml
│   │   │   ├── colors.xml
│   │   │   └── themes.xml
│   │   └── ...
│   └── AndroidManifest.xml
├── build.gradle
└── ...
```

## Key Components Used

- **BpkCardView**: Main container components with large corner styling
- **BpkText**: Text components with Backpack styling (Heading1, Body1)
- **ConstraintLayout**: Main layout container for positioning components
- **LinearLayout**: Vertical layout for organizing content within cards

## Customization

You can easily modify the app by:

- Changing airport codes in `activity_main.xml`
- Updating flight times
- Modifying the flight number
- Adjusting colors in `colors.xml`
- Changing themes in `themes.xml`

## Troubleshooting

- **Backpack components not displaying**: Ensure you're not using Android Studio Dolphin
- **Gradle sync issues**: Check your internet connection and try "File > Invalidate Caches and Restart"
- **Emulator issues**: Consult Android Studio's troubleshooting guide for emulator problems

## Dependencies

- Backpack Android UI Library: 43.0.0
- AndroidX Core KTX: 1.12.0
- AndroidX AppCompat: 1.6.1
- Material Design Components: 1.11.0
- ConstraintLayout: 2.1.4

## License

This project is created for educational purposes as part of the Android development task.
