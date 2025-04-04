# Project Structure - Part 4

### 6. Helper Components

#### Language Management and Translation
The app supports both Arabic and English languages:
- **Built-in Translation System**: Translate all UI text
- **Automatic Switching**: Adapt UI according to device language
- **Date and Time Formatting**: Display dates and times in appropriate format for the language

#### User Notifications (SnackBar)
System for displaying confirmation and error messages to the user:
- **Success Messages**: Confirm successful completion of operations
- **Error Messages**: Inform user of any issues
- **Customize Appearance**: Change color and shape of notifications based on message type

### 7. Data and Event Flow

#### Adding a New Medication:
1. User enters medication data in the add screen
2. A new Pill object is created with all information
3. The medication is stored in the database via the repository
4. A notification is scheduled for the medication time
5. User is redirected to the home screen

#### Editing an Existing Medication:
1. User selects a medication from the list and opens the edit screen
2. Current medication data is displayed in the form
3. User updates the required information
4. Pill object is updated with new data
5. Database is updated via the repository
6. Old notifications are canceled and new ones are scheduled

#### Logging Medication Intake:
1. User presses the "Taken" button on home screen
2. The lastTaken map in the Pill object is updated
3. Database is updated with the new information
4. A confirmation message is displayed to the user