# Water Girl Event Management App

## Overview

Water Girl is a Flutter-based mobile application designed for efficient event management. It provides features for attendee registration, QR code scanning, and real-time attendance tracking.

## Key Features

### 1. Authentication
- Secure login and signup functionality
- Persistent login state using SharedPreferences
- Automatic session refresh and logout on app resume

### 2. Dashboard
- Central hub with navigation to all main features
- Bottom navigation bar for easy access to different sections
- App bar with refresh and logout options

### 3. Attendee List Management
- View and manage a list of all registered attendees
- Search functionality to quickly find attendees by name or email
- Sort attendees alphabetically by name
- Create unique IDs (UIDs) for attendees without existing UIDs

### 4. QR Code Registration
- Scan QR codes to register new attendees or update existing ones
- Real-time UID assignment and database update
- Prevent duplicate UID assignments
- Toggle torch and switch camera options for better scanning

### 5. Attendance Tracking
- Scan attendee QR codes to mark attendance
- Real-time updates of check-in/check-out status
- View attendee details upon successful scan
- Manually toggle and confirm attendance status

### 6. Search Functionality
- Search through the entire attendee database
- Filter results by name or email
- Real-time search updates as you type
- Mark attendees as present or absent directly from search results

### 7. Theming
- Support for both light and dark themes
- Automatic theme switching based on system settings

### 8. Data Management
- Real-time synchronization with Supabase backend
- Efficient data fetching and caching for improved performance

## Technical Details

- Built with Flutter for cross-platform compatibility
- Uses Supabase for backend services and real-time database
- Implements MobileScannerController for QR code scanning
- Utilizes SharedPreferences for local data storage
- Follows Material Design principles for UI/UX

## Getting Started

1. Clone the repository
2. Set up your Supabase project and update the credentials in `main.dart`
3. Run `flutter pub get` to install dependencies
4. Launch the app using `flutter run`

## Dependencies

- flutter
- supabase_flutter
- shared_preferences
- mobile_scanner