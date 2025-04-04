# Project Structure - Medication Management App

## Overview
This application is a comprehensive medication management system designed to help users track their medications and schedule notifications for dose reminders. The app features a bilingual user interface (Arabic and English) and a robust data structure.

## Key Application Components

### 1. File Structure
The application is organized into functional folders following the standard design pattern for Flutter applications:

```
lib/
├── database/           # Database layer
│   ├── pills_database.dart     # SQLite database implementation
│   └── repository.dart         # Repository pattern for operation management
├── helpers/            # Helper functions
│   └── snack_bar.dart          # Display notifications to user
├── models/             # Data models
│   ├── medicine_type.dart      # Different medicine types
│   └── pill.dart               # Main medicine model
├── notifications/      # Notification system
│   └── custom_notification_service.dart  # Custom notification service
├── screens/            # Application screens
│   ├── add_new_medicine/       # Add new medicine
│   ├── edit_medicine/          # Edit medicine details
│   └── home/                   # Home screen
└── main.dart           # Application entry point
```