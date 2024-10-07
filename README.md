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

## How to Use

### 1. Login
- Launch the app and enter your credentials on the login screen.
- If you don't have an account, contact the system administrator for registration.

### 2. Dashboard Navigation
- Use the bottom navigation bar to switch between main features:
  - Attendee List (left icon)
  - Search (middle icon)
  - QR Scanner (right icon)

### 3. Managing Attendees
- On the Attendee List screen:
  - Scroll through the list of attendees.
  - Use the search bar at the top to find specific attendees.
  - For attendees without a UID, tap "Create UID" to assign one using QR code.

### 4. Registering New Attendees
- Navigate to the QR Scanner screen.
- Scan the attendee's QR code.
- If the attendee is not in the system, you'll be prompted to add their details.
- Confirm the information and save to register the new attendee.

### 5. Marking Attendance
- On the QR Scanner screen, scan an attendee's QR code.
- The attendee's information will appear on the screen.
- Use the "Present" or "Absent" button to set their status.
- Tap "Confirm" to save the attendance status.

### 6. Searching Attendees
- Go to the Search screen using the middle icon in the bottom navigation.
- Type a name or email in the search bar.
- Results will update in real-time as you type.
- Use the buttons next to each attendee to quickly mark them as present or absent.

### 7. Refreshing Data
- To refresh the current screen's data, tap the refresh icon in the top-right corner of the app bar.

### 8. Logging Out
- To log out, tap the logout icon in the top-right corner of the app bar.

### Tips
- Ensure good lighting when scanning QR codes for best results.
- You can toggle the flashlight on/off and switch cameras while scanning QR codes.
- The app will automatically adjust to your device's light/dark mode settings.
- Internet connection is required for real-time updates and synchronization.

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