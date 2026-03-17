# University Timetable Management System

This project is a full-stack web application designed to collaboratively manage a university faculty's timetable. The system centralizes resources such as classrooms, professors, and student groups, and prevents human errors by automatically detecting scheduling conflicts in real-time.

## User Roles:
*   **Administrator**: Manages core data like classrooms, professors, subjects, and student groups, with full editing rights over the entire timetable.
*   **Professor**: Authenticated users who can schedule their own teaching activities (lectures, labs, seminars) in available slots. They can only edit or delete their own entries.
*   **Student / Visitor**: Has "read-only" access, allowing them to view the timetable filtered by student group, classroom, or professor, without the ability to modify any data.

## Key Features (Minimum Viable Product):
*   **Resource Management (CRUD)**: An interface for administrators to configure basic entities: classrooms (name, capacity, type, facilities), professors (identification data, department), student groups (identifier, year, series), and subjects (name, activity type).
*   **Conflict Detection Engine**: An automatic validation system that runs every time an activity is scheduled. An activity is saved only if it passes checks for classroom availability, student group availability, and professor availability.
*   **Tabular Timetable View**: The main display interface, organized as a matrix (Monday-Friday, 2-hour time slots), showing dynamic data (subject, professor, classroom) with color codes to differentiate activity types (e.g., Lecture - Yellow, Lab - Blue).
*   **Filtering and Search System**: Allows users to isolate relevant information by filtering by student group, professor, or classroom.
*   **Authentication and Security**: A login system for administrators and professors, with role-based access control to ensure professors cannot modify entries made by other colleagues.
