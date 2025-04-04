# Project Structure - Part 2

### 2. Data Model

#### Pill Model
This model represents a single medication and contains:
- **id**: Unique identifier for each medication
- **name**: Name of the medication
- **description**: Description including dosage and medicine type
- **color**: Visual color to distinguish the medication
- **times**: List of TimeOfDay objects representing times to take the medication
- **days**: List of numbers representing days of the week when the medication is taken
- **isActive**: Indicates whether medication reminders are active
- **lastTaken**: Map recording the last time the medication was taken
- **notificationDate**: Date and time for the next notification

#### MedicineType Model
This model represents different types of medicines (pills, capsules, syrup, etc.) with:
- **name**: Name of the medicine type in English
- **arabicName**: Name of the medicine type in Arabic
- **medicineTypes**: Predefined list of all supported medicine types

### 3. Database Layer

#### PillsDatabase
Manages the local database using SQLite with:
- **Create Pills Table**: Defines pills table structure in the database
- **CRUD Operations**: Add, read, update, and delete pill data
- **Data Processing**: Convert between Dart models and database formats
- **Time Storage**: Store pill times as JSON string in the database
- **Day Storage**: Store days of the week as JSON string in the database

#### Repository
Serves as an interface between the UI layer and the database:
- **Database Abstraction**: Hides database implementation details
- **Data Synchronization**: Ensures data consistency across the app
- **Business Operations**: Contains business logic for complex operations