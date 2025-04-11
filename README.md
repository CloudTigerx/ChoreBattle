# Chore Battle

A gamified chore management app built with Flutter and GetX.

## Features

- Gamified chore management system
- Point-based reward system
- Competitive leaderboard
- Task tracking and completion
- User profiles and achievements
- Image upload and storage
- Google authentication
- Local notifications
- Offline data persistence

## Tech Stack

- **Flutter**: Cross-platform UI framework
- **GetX**: State management, routing, and dependency injection
- **Firebase**: Backend services (Storage)
- **Google Sign In**: Authentication
- **Local Storage**: Shared Preferences

## Getting Started

### Prerequisites

- Flutter SDK (3.29.2 or higher)
- Git
- Android Studio / VS Code with Flutter extensions
- Firebase account and project
- Google Cloud project (for authentication)

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/chore_battle.git
```

2. Navigate to the project directory:
```bash
cd chore_battle
```

3. Install dependencies:
```bash
flutter pub get
```

4. Configure Firebase:
   - Create a new Firebase project at [Firebase Console](https://console.firebase.google.com)
   - Add Android/iOS apps to your Firebase project
   - Download and add configuration files:
     - Android: Place `google-services.json` in `android/app/`
     - iOS: Place `GoogleService-Info.plist` in `ios/Runner/`

5. Run the app:
```bash
flutter run
```

## Project Structure

```
lib/
├── controllers/     # GetX controllers
├── models/         # Data models
├── views/          # UI screens
├── routes/         # GetX routes
├── services/       # Business logic
└── utils/          # Helper functions
```

## Dependencies

Main dependencies include:

```yaml
dependencies:
  # Firebase
  firebase_core: ^2.27.1
  firebase_storage: ^11.6.10
  
  # Authentication
  google_sign_in: ^6.2.1
  
  # Storage and preferences
  shared_preferences: ^2.2.2
  
  # UI and utilities
  image_picker: ^1.0.7
  flutter_svg: ^2.0.10+1
  flutter_local_notifications: ^16.3.2
```

## GetX Implementation

This project uses GetX for:
- State Management
- Navigation
- Dependency Injection
- Internationalization
- Theme Management

### Key GetX Features Used

- `GetMaterialApp`: Enhanced MaterialApp with GetX features
- `GetX` and `Obx`: Reactive state management
- `Get.to()` and `Get.off()`: Navigation
- `Get.put()`: Dependency injection
- `.tr`: Translation support

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Flutter team for the amazing framework
- GetX team for the powerful state management solution
- Firebase team for the backend services
- All contributors and supporters 