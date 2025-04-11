# Chore Battle

A gamified chore management app built with Flutter and GetX.

> **Note**: This is a private repository. Access is limited to authorized contributors only.

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

## Project Structure

The project follows a clean, modular architecture with clear separation of concerns:

```
lib/
├── controllers/     # GetX controllers for state management
├── models/         # Data models and business logic entities
├── views/          # UI screens and widgets
├── routes/         # GetX route management and navigation
├── services/       # Business logic and external service integration
└── utils/          # Helper functions and utilities
```

### Directory Structure Explanation

- **controllers/**: Contains GetX controllers that manage the state and business logic of the app. Each controller is responsible for a specific feature or screen.
- **models/**: Houses data models that represent the core entities of the application (users, chores, rewards, etc.).
- **views/**: Contains all UI-related code, organized by feature. Each screen has its own directory with associated widgets.
- **routes/**: Manages navigation and routing using GetX, making it easy to navigate between screens while maintaining state.
- **services/**: Handles external service integration (Firebase, local storage) and complex business logic.
- **utils/**: Contains reusable utility functions, constants, and helper classes.

## Version Control

This project uses Git for version control. The repository is structured to:
- Track all source code changes
- Ignore build artifacts and sensitive files (see `.gitignore`)
- Maintain empty directories using `.gitkeep` files
- Follow Git best practices for Flutter development

### Branching Strategy

We follow a modified Git Flow workflow with the following branches:

#### Main Branches
- `master` - Production-ready code
- `develop` - Main development branch, feature branches merge here

#### Supporting Branches
- `feature/*` - New features and non-emergency bug fixes
- `bugfix/*` - Bug fixes for develop branch
- `hotfix/*` - Emergency production fixes
- `release/*` - Release preparation

### Branch Naming Convention
- Feature branches: `feature/feature-name`
- Bug fixes: `bugfix/bug-name`
- Hotfixes: `hotfix/issue-name`
- Releases: `release/version-number`

### Workflow Rules
1. **Feature Development**
   - Create from: `develop`
   - Merge back into: `develop`
   - Naming: `feature/feature-name`

2. **Bug Fixes**
   - Create from: `develop`
   - Merge back into: `develop`
   - Naming: `bugfix/bug-name`

3. **Hotfixes**
   - Create from: `master`
   - Merge back into: `master` and `develop`
   - Naming: `hotfix/issue-name`

4. **Releases**
   - Create from: `develop`
   - Merge back into: `master` and `develop`
   - Naming: `release/version-number`

### Commit Guidelines
- Use clear, descriptive commit messages
- Start with a verb in imperative mood (e.g., "Add", "Fix", "Update")
- Reference issue numbers when applicable
- Keep commits focused and atomic

### Pull Request Process
1. Create PR from your feature branch to `develop`
2. Ensure tests pass and code is reviewed
3. Squash and merge when approved
4. Delete feature branch after merge

## Getting Started

### Prerequisites

- Flutter SDK (3.29.2 or higher)
- Git
- Android Studio / VS Code with Flutter extensions
- Firebase account and project
- Google Cloud project (for authentication)

### Installation

1. Clone the repository (requires access):
```bash
git clone https://github.com/CloudTigerx/ChoreBattle.git
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