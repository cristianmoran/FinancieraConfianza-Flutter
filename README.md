# financiera_confianza

A new Flutter project.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://flutter.dev/docs/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://flutter.dev/docs/cookbook)

For help getting started with Flutter, view our
[online documentation](https://flutter.dev/docs), which offers tutorials,
samples, guidance on mobile development, and a full API reference.


Para ejecutar la aplicacion se utilizan dart define y flavors
ENVIRONMENT DEV:
//IOS
flutter run --{BUILD_TYPE}

//ANDROID
flutter run --{BUILD_TYPE}
flutter run --profile --flavor dev -t lib/main.dart
flutter run --release --flavor dev -t lib/main.dart

ENVIRONMENT PROD:
//IOS PROD
flutter run --dart-define=DEFINECONFIANZA_APP_NAME=FinancieraConfianza --dart-define=DEFINECONFIANZA_APP_SUFFIX= -t lib/main_ios.dart (PROD)
flutter run --release --dart-define=DEFINECONFIANZA_APP_NAME=FinancieraConfianza --dart-define=DEFINECONFIANZA_APP_SUFFIX= -t lib/main_ios.dart (PROD)

//Android PROD
flutter run --flavor prod --dart-define=DEFINECONFIANZA_APP_NAME=FinancieraConfianza -t lib/main.dart (PROD)
flutter run --profile --flavor prod --dart-define=DEFINECONFIANZA_APP_NAME=FinancieraConfianza -t lib/main.dart (PROD)
flutter run --release --flavor prod --dart-define=DEFINECONFIANZA_APP_NAME=FinancieraConfianza -t lib/main.dart (PROD)

BUILD APK
//Android
    - Dev
flutter build apk --debug --flavor dev -t lib/main.dart
flutter build apk --profile --flavor dev -t lib/main.dart
flutter build apk --release --flavor dev -t lib/main.dart
    -Prod
flutter build apk --release --flavor prod -t lib/main.dart --dart-define=DEFINECONFIANZA_APP_NAME=FinancieraConfianza

flutter build appbundle --release --flavor prod -t lib/main.dart --dart-define=DEFINECONFIANZA_APP_NAME=FinancieraConfianza

