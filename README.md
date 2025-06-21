# JavaGymManagement

A comprehensive gym management system built with Java Swing and MySQL, designed to streamline gym operations through separate admin and student portals.

## Overview

JavaGymManagement is a desktop application that provides a complete solution for managing gym members, equipment, queries, and user authentication. The system features role-based access with distinct interfaces for administrators and students, enabling efficient gym operations and member engagement.

## Features

### Admin Portal
- **Member Management**: Add, edit, and delete gym members with comprehensive profile information
- **Equipment Management**: Track and update gym equipment inventory and availability
- **Query Management**: View member complaints/suggestions and send responses
- **User Authentication**: Manage user credentials and password resets
- **Database Integration**: Full CRUD operations with MySQL database

### Student Portal
- **Workout Timer**: Built-in timer functionality for tracking workout sessions
- **Equipment Viewing**: Real-time access to equipment availability
- **Query System**: Submit complaints, suggestions, and feedback
- **Member Directory**: View other gym members and their departments
- **Reply System**: Check responses from administration

### Authentication System
- **Secure Login**: Username/password authentication with database validation
- **Password Recovery**: Security key-based password reset functionality
- **Role-based Access**: Separate access levels for admin and student users

## Project Structure

```
JavaGymManagement/
├── mod1/               # Authentication Module
│   ├── loginf.java     # Main login interface
│   ├── resetpassword.java    # Password reset (step 1)
│   └── resetpassword2.java   # Password reset (step 2)
├── mod2/               # Admin Module
│   ├── home.java       # Admin dashboard
│   ├── member.java     # Member management
│   ├── adminquery2.java     # Query response system
│   ├── queryview.java  # View received queries
│   └── updequip.java   # Equipment management
├── mod3/               # Student Module
│   ├── student2.java   # Student dashboard
│   ├── objective.java  # Workout timer
│   ├── equipments.java # Equipment viewing
│   ├── studentquery.java    # Query submission
│   └── replyad.java    # View admin replies
└── mod4/               # Additional Features
    ├── setpassw.java   # Password management
    └── viewmembers.java     # Member directory
```

## Technology Stack

- **Language**: Java 8+
- **GUI Framework**: Java Swing with NetBeans Form Designer
- **Database**: MySQL 8.0
- **IDE**: NetBeans IDE
- **Additional Libraries**: 
  - JCalendar (for date selection)
  - MySQL Connector/J (JDBC driver)

## Database Schema

The system uses MySQL with the following key tables:

- **users**: Authentication credentials and security keys
- **members**: Gym member profiles and information
- **equipments**: Equipment inventory and availability
- **complaint**: Member queries and suggestions
- **addressals**: Admin responses to queries

## Installation & Setup

### Prerequisites
- Java JDK 8 or higher
- NetBeans IDE (recommended)
- MySQL Server 8.0+
- MySQL Connector/J driver

### Database Setup
1. Create a MySQL database named `db1`
2. Update database connection parameters in each module:
   - Host: `localhost:3306`
   - Username: `root`
   - Password: Update in connection strings

### Running the Application
1. Open the project in NetBeans IDE
2. Ensure MySQL server is running
3. Update database connection credentials in source files
4. Build and run the project
5. Default admin credentials: `admin` / `12345`

## Key Functionalities

### Member Management
- Store comprehensive member information including student ID, name, year of study, department, hostel, and joining date
- Real-time table updates with add, edit, delete operations
- Data validation and error handling

### Equipment Tracking
- Maintain equipment inventory with availability counts
- Real-time updates across admin and student interfaces
- Equipment addition, modification, and removal capabilities

### Communication System
- Bidirectional communication between students and administration
- Query categorization and response tracking
- Notification system for new queries and responses

### Timer Functionality
- Built-in workout timer with start/stop controls
- Session tracking for student workout monitoring
- Simple and intuitive interface design

## Security Features

- Password-based authentication with database validation
- Security key system for password recovery
- Role-based access control preventing unauthorized access
- SQL injection prevention through prepared statements

## User Interface

The application features a modern Java Swing interface with:
- Consistent color scheme (black headers with blue/purple accents)
- Intuitive navigation between modules
- Responsive table components for data display
- Form validation and user feedback
- Professional layout with proper spacing and alignment

## Future Enhancements

- Payment processing integration
- Membership plan management
- Attendance tracking system
- Reporting and analytics dashboard
- Mobile application companion
- Backup and restore functionality

## Contributing

This project follows standard Java development practices with clear module separation and consistent coding standards. When contributing:

1. Maintain the existing code structure
2. Follow Java naming conventions
3. Update database connections as needed
4. Test all CRUD operations thoroughly
5. Ensure UI consistency across modules