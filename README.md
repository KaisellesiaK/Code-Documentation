# PhilTech School Management System Documentation

## Overview
A console-based school management system with user roles, enrollment, attendance tracking, and EOG request management.

## Core Features
- User authentication with multiple roles
- Student enrollment management  
- Attendance tracking
- EOG (End of Grade) request processing
- Subject management

## User Roles
1. Student
   - Can enroll in courses
   - View subjects
   - Request EOG documents

2. Teacher  
   - Manage classroom
   - Mark/view attendance
   - View course details

3. Administrator
   - Manage enrollees
   - Process EOG requests 
   - Classroom oversight

4. Registrar
   - Manage enrollees
   - Manage subject tables
   - Process EOG requests

## Key Functions

### Authentication
- `loadUsers()` - Loads user data from file
- `saveUsers()` - Saves user data to file
- `login()` - Handles user authentication
- `signup()` - New user registration

### Enrollment
- `viewEnrollees()` - Display enrolled students
- `deleteEnrollee()` - Remove student from course
- `saveEOGRequest()` - Save certification/clearance requests

### Attendance
- Record daily attendance 
- View attendance history
- Generate attendance reports

### Data Files
- users.txt - User credentials and roles
- {course}_enrollees.txt - Course enrollment data
- attendance_{teacher}_{subject}.txt - Attendance records
- certification_requests.txt - EOG certification requests
- clearance_requests.txt - EOG clearance requests

## Usage
1. Run the program
2. Login with credentials or signup
3. Access role-specific menu
4. Perform allowed operations
5. Logout when done

## Notes
- All data is persistently stored in text files
- Input validation implemented for data integrity
- Console-based UI with simple navigation
