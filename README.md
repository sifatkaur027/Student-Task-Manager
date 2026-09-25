# Student-Task-Manager
The Student Task Manager is a simple Python-based task management system designed to help students organize and manage their daily tasks. The program allows users to add tasks, view all tasks, mark tasks as completed, filter tasks according to priority, and delete tasks. 
Features
•	Add a new task
•	Assign a priority to each task:
o	High
o	Medium
o	Low
•	View all saved tasks
•	Mark a task as completed
•	Filter tasks by priority
•	Delete a task
•	Automatically generate unique task IDs
•	Save tasks permanently in tasks.txt
•	Load previously saved tasks when the program starts
•	Handle invalid user input

 Technologies Used
•	Python 3
•	File Handling
•	Lists
•	Dictionaries
•	Functions
•	Loops
•	Conditional Statements
•	Exception Handling
•	String Manipulation

Project Structure
Student-Task-Manager
 student_task_manager.py
 tasks.txt
 README.md
Files
student_task_manager.py
Contains the complete Python source code for the Student Task Manager.
tasks.txt
Stores task information permanently.
README.md
Contains information about the project, its features, and how to use it.

 How to Run
1. Install Python
Make sure Python 3 is installed on your computer.
You can check the installed version using:
python --version
2. Save the Program
Save the Python code as:
student_task_manager.py
3. Run the Program
Open the terminal in the project folder and run:
python student_task_manager.py
The program will display the Student Task Manager menu.

Main Menu
When the program runs, the following menu is displayed:
STUDENT TASK MANAGER SYSTEM
1. Add New Task
2. View All Tasks
3. Mark Task as Complete
4. Filter Tasks by Priority
5. Delete Task
6. Exit

How to Use
1. Add New Task
Select option 1.
Enter the task title and choose a priority:
Enter task title: Complete Python Assignment

Select Priority Level:
1. High
2. Medium
3. Low

Enter choice (1-3): 1
The task will be created with the status:
Pending

2. View All Tasks
Select option 2.
The program displays all tasks in the following format:
ID   | Priority | Status | Task Title

1    | High     | Pending     | Complete Python Assignment
2    | Medium   | Completed   | Study Mathematics
3    | Low      | Pending     | Submit Project

3. Mark Task as Complete
Select option 3.
Enter the ID of the task that you have completed.
For example:
Enter Task ID to mark as Completed: 1
The task status changes from:
Pending
to:
Completed

4. Filter Tasks by Priority
Select option 4.
Choose one of the available priorities:
1. High
2. Medium
3. Low
The program will display only the tasks having the selected priority.

5. Delete Task
Select option 5.
Enter the ID of the task you want to delete:
Enter the ID of the task to delete: 2
The selected task will be removed from the task list and the updated data will be saved to the file.

6. Exit
Select option 6 to exit the program.
The program ends and the task data remains saved in tasks.txt.

Data Storage
The program uses a text file named:
tasks.txt
Each task is stored in the following format:
ID | Title | Priority | Status
For example:
1|Complete Python Assignment | High | Pending
2|Study Mathematics | Medium | Completed
3|Submit Project | Low | Pending
The | symbol separates the different pieces of task information.

 Functions Used
Function	Purpose
load_tasks()	Loads tasks from tasks.txt
save_tasks_to_file()	Saves tasks to tasks.txt
add_task()	Creates and adds a new task
view_all_tasks()	Displays all tasks
delete_task()	Deletes a task using its ID
mark_task_complete()	Marks a task as completed
filter_by_priority()	Displays tasks according to priority
main()	Controls the main menu and program flow

 Python Concepts Demonstrated
This project demonstrates several fundamental Python programming concepts:
Lists
A list is used to store all tasks in memory:
tasks = []
Dictionaries
Each task is represented using a dictionary:
{"id": 1,
  "title": "Complete Assignment",
  "priority": "High",
  "status": "Pending"}
Functions
The program is divided into multiple functions to make the code organized and reusable.
File Handling
The program uses file operations to permanently store data:
open()
readlines()
write()
close()
Loops
for and while loops are used to process tasks and repeatedly display the menu.
Conditional Statements
if, elif, and else statements are used to make decisions based on user input.
Exception Handling
try-except is used to handle invalid numerical input and missing files.

Program Flow
Start - Load tasks from tasks.txt
  ↓
Display Main Menu
  ↓
User selects an option
  ↓
Perform selected operation
  ↓
Save changes if required
  ↓
Return to Main Menu
  ↓
User selects Exit
  ↓
End

Input Validation
The program checks for several types of invalid input.
Examples:
•	Empty task titles are rejected.
•	Invalid priority choices are rejected.
•	Non-numerical task IDs are handled.
•	Invalid menu choices are rejected.
•	A task ID that does not exist produces an error message.

 Objective
The main objective of this project is to demonstrate how basic Python programming concepts can be combined to create a practical application.
It provides students with experience in:
•	Problem solving
•	Functions
•	Data structures
•	File handling
•	User input
•	Exception handling
•	Basic application design
 Future Improvements
The project can be extended by adding:
•	Edit/update task functionality
•	Search tasks by title
•	Due dates
•	Sorting tasks by priority
•	Task categories
•	Automatic overdue-task detection
•	A graphical user interface (GUI)
•	Database storage using SQLite
•	User login and multiple student accounts

 Conclusion
The Student Task Manager is a beginner-friendly Python application that provides basic task management functionality while demonstrating important programming concepts such as lists, dictionaries, functions, file handling, loops, conditional statements, and exception handling.
It can serve as a foundation for developing a more advanced task management application in the future.

