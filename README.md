# Instagram Clone — Flutter Social Media App

A responsive social media app built with Flutter and Firebase. It supports Android and web, with an iOS project also included.

## Features

- Email and password sign-up and login
- Create posts with a photo and caption
- View posts and like or comment on them
- Search for users and follow or unfollow them
- View profiles, posts, followers, and following
- Real-time data updates with Cloud Firestore

## Tech stack

- Flutter and Dart
- Firebase Authentication
- Cloud Firestore
- Firebase Storage
- Provider

## Getting started

### Requirements

- Flutter SDK with Dart 2.x (the project currently requires Dart `>=2.15.0 <3.0.0`)
- A configured Firebase project
- Chrome for running the web app, or an Android device/emulator

> Recent Flutter releases bundle Dart 3, which does not satisfy the current SDK constraint. Use a Flutter release with Dart 2.x, or update the project and dependencies to support Dart 3.

### Install dependencies

From the project directory, run:

```powershell
flutter doctor
flutter pub get
flutter devices
```

### Run the app

Run in Chrome:

```powershell
flutter run -d chrome
```

Run on a connected Android device or emulator:

```powershell
flutter run
```

Building or running the iOS app requires macOS and Xcode.

## Firebase configuration

Create a Firebase project and register an app for each platform you intend to run. Enable Email/Password sign-in, configure Cloud Firestore and Firebase Storage, and set secure Firestore and Storage rules.

- **Web:** Update the `FirebaseOptions` in `lib/main.dart` with your web app's Firebase configuration.
- **Android:** Add your Firebase Android configuration as `android/app/google-services.json`.
- **iOS:** Add your Firebase iOS configuration as `ios/Runner/GoogleService-Info.plist`.

Never add Firebase Admin SDK service-account keys or other private credentials to the repository.

## Acknowledgements

This project is based on the [Flutter Instagram Clone](https://github.com/RivaanRanawat/instagram-flutter-clone) by Rivaan Ranawat and its [YouTube tutorial](https://youtu.be/BBccK1zTgxw).
