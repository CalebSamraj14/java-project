
##Student Management System#


Overview

The Student Management System is a console application built in Java that efficiently manages student records. Users can perform CRUD (Create, Read, Update, Delete) operations on student data. The system features functionalities for adding, viewing, updating, deleting, and searching for students, as well as generating reports. It also ensures data persistence, allowing student records to be saved and reloaded across different application sessions.

#Features

Add New Student:

Users can add a new student record by entering the roll number, name, course, and marks.

#View All Students:

This feature displays a comprehensive list of all student records along with their details.

#Update Student Information:

Users can modify an existing student’s name, course, or marks by using their roll number.

#Delete Student Record:

This option allows users to remove a student record from the system using the roll number.

#Search for Student:

Users can search for a student by roll number or name, and the system will display their information if found.

#Generate Reports:

The system calculates and presents a report that includes the total number of students, total marks, and average marks.

#Data Persistence:

All student records are stored in a file (students.dat) to ensure that data is preserved even after the application is closed.

#Code Explanation

1. Main Class
2. 
The Main class contains the main method, which acts as the entry point for the application. It manages the user interface and menu options.

3. Student Class
4. 
The Student class serves as a model for student records. It includes:

Fields: rollNumber, name, course, and marks.

Getters and setters for encapsulating the data.

A toString method for displaying student details.

3. Menu Options
   
The program presents a menu with options (1-7) for various features. The user selects an option, and the corresponding method is executed.

5. Methods
   
addNewStudent()

Prompts the user to enter the roll number, name, course, and marks of a new student.
Creates a Student object and adds it to the list of students.

viewAllStudents()

This function goes through the list of students and displays all their records.
It also takes care of situations where the list might be empty.

updateStudent()

This function looks for a student using their roll number.
It prompts the user to update the student's name, course, or marks.

deleteStudent()

This function searches for a student by their roll number.
If the student is found, it removes them from the list.

searchStudent()

This function allows the user to find a student by either roll number or name.
It shows the details of the student that matches the search criteria.

generateReport()

This function calculates the total number of students, their total marks, and the average marks.
It presents the report in a format that is easy to understand.

saveStudents()

This function uses ObjectOutputStream to serialize the list of students and save it to a file named students.dat.

loadStudents()

This function uses ObjectInputStream to deserialize and load the list of students from the file when the program starts.

#Usage

To use the program, run it and select an option from the menu.
Follow the prompts to add, update, or view student information.
You can exit the program using option 7, and your data will be saved automatically.
Technologies Used

Language: Java
Persistence: Serialization (File I/O)
Data Structures: ArrayList
How to Run

Compile the program with javac Main.java.
Run it using java Main.
Interact with the menu options as needed.


##Sample Output
Student Management System
1. Add New Student
2. View All Students
3. Update Student Information
4. Delete Student Record
5. Search for Student
6. Generate Report
7. Exit
Enter your choice:

