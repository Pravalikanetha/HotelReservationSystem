Hotel Reservation System

This Java program implements a command-line interface for a hotel reservation system, allowing users to manage reservations through a MySQL database.

Key Features:

Reservation Management:

Create new reservations by specifying guest name, room number, and contact information.
View existing reservations with details like guest name, room number, contact details, and reservation date.
Retrieve the room number for a specific reservation by providing the reservation ID and guest name (for security purposes).
Update existing reservations by entering the reservation ID, followed by changes to guest name, room number, or contact details.
Delete reservations by providing the reservation ID (confirmation prompt is recommended).
Database Interaction:

Connects to a MySQL database (named hotel_db by default) using JDBC.
Executes SQL queries to interact with the reservations table.
Error Handling:

Catches and provides informative messages for potential exceptions like SQLException.
Basic Input Validation:

Validates user input for numeric fields (reservation ID, room number) to prevent unexpected behavior.
Room for Improvement:

Security:
Consider storing database credentials in environment variables or a secure configuration file instead of hardcoding them in the program.
Implement prepared statements to prevent SQL injection vulnerabilities.
User Authentication:
Add a user authentication system to restrict unauthorized access to reservations (optional, based on your requirements).
User Interface:
Explore a more user-friendly interface in the future (e.g., GUI or web application) to enhance user experience.
Getting Started

Prerequisites:

Java Development Kit (JDK) installed
MySQL database server running
MySQL JDBC driver (included in most Java distributions)
Configuration:

Update the url, username, and password variables in the HotelReservationSystem class to match your MySQL database connection details.
Create the hotel_db database and a table named reservations with appropriate columns (e.g., reservation_id, guest_name, room_number, contact_number, reservation_date).
Compilation and Execution:

Compile the program using a Java compiler (e.g., javac HotelReservationSystem.java).
Run the program using java HotelReservationSystem.
Example Usage

The program presents a menu with options for managing reservations. Refer to the program code for specific prompts and input formats.

Additional Notes:

This is a basic implementation for educational purposes. Consider extending it to meet your specific hotel reservation system requirements.
Feel free to adapt the code to your database schema and preferences.
