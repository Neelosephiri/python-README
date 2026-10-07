# README.md 
students= {}
num_students = int(input('How many students do you want to enter?'))
for i in range(num_students):
    name = input("Enter student name: ")
    student_grades = {}
    for subject in ["Math", "English", "Science"] :
        grade = float(input("Enter" + subject +"grade:"))
        while grade <0 or grade>100 :
            print("Invalid grade. Please enter a garade between 0 and 100.")
        student_grades[subject] = grade
        students[name] = student_grades
print("\nUPADATE STUDENT")
name = input("Which subject do you want to update?")
if name in students:
    subject = input("Which subject do you want update?")
    if subject in students[name]:
        grade = float(input("Enter new grade:"))
    while grade <0 or grade >100:
        print("Invalid grade.Please enter a grade between 0 and 100.")
        grade= float(input("Enter new grade:"))
        students[name][subject]=grade
    else
        print ("Subject not found.")
print("\nREMOVE STUDENT")
name = input("Enter student's name:")
if name in students:
    del students[name]
    print("Student removed.")
else
    print ("Student not found.")

print("\nVIEW SUBJECT GRADES")
subject= input('Enter subject:')
for name, grades in students.items():
    if subject in grades :
        print(name, ":", grades[subject])

print("/nSEARCH STUDENT")
name= input("Enter student's name :")

if name in students:
    grades= students[name]
    total = sum.(grades.values())
    average= total/ len(grades)
    print ("Name:", name)
    print("Grades:", grades
    print("Average:", average)
else
    print("Student not found.")


Section A - Gradebook Management System

The Gradebook Management System allows the user to enter and manage student grades. The user first enters the number of students, followed by each student’s name and grade.

The program verifies each grade to make sure it is between 0 and 100. If an invalid grade is entered, the user is asked to enter it again. The student names and grades are then stored in a list.

After entering the grades, the program calculates the class total and class average and displays the student names, grades, total, and average.

Main Features

* Accepts the number of students.
* Records each student’s name and grade.
* Validates grades between 0 and 100.
* Stores student information.
* Calculates the class total and average.
* Displays the student grades and class results.

Python Concepts Used

The system uses variables, lists, tuples, loops, user input, while loops, validation, and arithmetic calculations.

Section C - Gradebook Management System

The Gradebook Management System is used to record and analyse student grades. The user enters the number of students and then enters each student’s name and grades for Math, English, and Science.

The program verifies each grade to make sure it is between 0 and 100. The grades are stored together with each student’s name.

The system calculates and displays each student’s average grade. It also finds and displays the highest and lowest grade for each subject.

Main Features

* Allows the user to enter multiple students.
* Records grades for Math, English, and Science.
* Validates grades between 0 and 100.
* Stores student names and grades.
* Calculates each student’s average.
* Finds the highest and lowest grade for each subject.
* Displays the student results and grade analysis.

Python Concepts Used

The program uses variables, lists, tuples, loops, user input, conditional statements, validation, functions such as max() and min(), and arithmetic calculations.

Section C - Gradebook Management System

The Gradebook Management System allows the user to store and manage student grades for Math, English, and Science. The system uses a dictionary to store each student’s name and their subject grades.

The program allows the user to update a student’s grade, remove a student, view grades for a specific subject, and search for a student. When searching for a student, the system displays their grades and calculates their average.

The program also verifies grades to ensure they are between 0 and 100.

Main Features

* Stores multiple students and their subject grades.
* Allows grades to be updated.
* Allows students to be removed.
* Displays grades for a selected subject.
* Searches for a specific student.
* Calculates a student’s average grade.
* Validates grades between 0 and 100.

Python Concepts Used

The program uses dictionaries, lists, loops, conditional statements, user input, validation, dictionary methods, and arithmetic calculations.
