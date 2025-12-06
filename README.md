Student Management System (C Program)

This project is a simple console-based Student Management System written in C.
It supports user authentication with three roles — Admin, Staff, and Guest — and provides different access privileges for each.

The system stores student records in a text file and allows adding, updating, deleting, searching, and displaying students depending on user permissions.

🚀 Features
🔐 User Login

Users must log in using credentials stored in credentials.txt.
Each user has a role:

Admin

Add student

Display students

Search student

Update student

Delete student

Logout

Staff

Add

Display

Search

Update

Logout

Guest

Display

Search

Logout

📁 Files Used
1. credentials.txt

Stores login information in the format:

username password role


Example:

admin admin123 admin
teacher pass123 staff
viewer guest123 guest

2. students.txt

Stores student records.
(Depending on the improved code, it may use | as a delimiter.)

Format:

roll|name|mark


Example:

101|John Doe|88.50
102|Alice|91.00

🧩 Program Flow

Program starts → asks for USERNAME and PASSWORD

Checks credentials.txt

If login succeeds → loads menu based on role:

Admin Menu

Staff Menu

Guest Menu

User performs allowed operations on students.txt

User logs out

📚 Menu Options
Admin Menu
1. Add Student
2. Display Students
3. Search Student
4. Update Student
5. Delete Student
6. Logout

Staff Menu
1. Add Student
2. Display Students
3. Search Student
4. Update Student
5. Logout

Guest Menu
1. Display Students
2. Search Student
3. Logout

🛠️ Compilation & Running
Compile:
gcc main.c -o sms

Run:
./sms

📌 Requirements

GCC compiler

Basic knowledge of running console applications

Make sure the files credentials.txt and students.txt exist (or will be created on first write)

⚠️ Limitations

Text-file-based storage (no database)

No encryption for passwords

Basic input handling

No prevention for duplicate roll numbers

Designed for educational purposes only

📝 Recommended Improvements

If you want to enhance this program, consider:

Using structures (struct Student)

Switching to binary file storage

Adding password hashing

Adding input validation

Creating separate functions for file parsing
