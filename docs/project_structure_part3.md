# Project Structure - Part 3

### 4. Notifications System

#### CustomNotificationService
Provides an interface for managing medication notifications:
- **Schedule Notifications**: Create notifications at specified times
- **Cancel Notifications**: Remove existing notifications
- **Customize Notifications**: Set title, content, and sounds
- **Handle Permissions**: Request and manage notification permissions
- **Recurring Notifications**: Support for periodic notifications for recurring medications

### 5. Application Screens

#### Home Screen
Displays an overview of all scheduled medications:
- **Medication List**: Show all stored medications
- **Filter and Sort**: Options to filter and sort the medication list
- **Dose Logging**: Record the taking of medications
- **Quick Access**: Buttons to add new medications or edit existing ones

#### Add New Medicine Screen
Allows users to add new medications with:
- **Medication Data**: Enter medication name and description
- **Type Selection**: Select medicine type (pill, capsule, syrup, etc.)
- **Dosage Setting**: Set amount and unit of medication
- **Time Scheduling**: Choose time and date to take the medication
- **Recurrence**: Set number of weeks to repeat the medication

#### Edit Medicine Screen
Allows editing existing medication data:
- **Update Info**: Change medication name or dosage
- **Edit Times**: Change time or date to take medication
- **Edit Recurrence**: Change the weeks of repetition
- **Delete Medication**: Remove the medication completely from the system
- **Update Notifications**: Reschedule notifications based on changes