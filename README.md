# Employee Management System

A Python-based application designed to manage employee data for a company or organization efficiently. The system allows users to perform CRUD operations on employee records.

## Features

### 1. **Add Employee**

![Add Employee Screenshot](https://github.com/user-attachments/assets/901ce151-fed7-4564-83ca-393ffe13549a)

- **How it works:**
  - Takes employee details as input from the user.
  - Reads the employee file and checks if there are any employees.
  - If employees exist, the new employee will receive an ID one greater than the last employee in the file.
  - Saves the new employee details in the file.

### 2. **List Employees**

![List Employees Screenshot](https://github.com/user-attachments/assets/825a7840-214b-44e2-94c9-3e3e58a761ad)

- **How it works:**
  - Reads the employee file and stores its data in a list of strings.
  - Iterates over the list and displays the data on the console.

### 3. **Search for an Employee**

![Search Employee Screenshot](https://github.com/user-attachments/assets/a7a8c2a8-befa-4670-8623-fdc17d1fa524)

- **How it works:**
  - Reads the file and stores its data in a list of strings.
  - Iterates over the list and checks if the current ID matches the input ID.
  - If found, displays the employee data; otherwise, shows that the employee isn't found.

### 4. **Update Employee**

![Update Employee Screenshot](https://github.com/user-attachments/assets/ed048e5a-0bfe-4b74-ad5c-dcb292203aca)

- **How it works:**
  - Reads the file and stores its data in a list of strings.
  - Iterates through the list and finds the employee with the specified ID.
  - Prompts the user for the attribute they wish to update and its new value.
  - Updates the employee data and overwrites the file.

### 5. **Delete Employee**

![Delete Employee Screenshot 1](https://github.com/user-attachments/assets/b8b29e5a-f512-4ce4-9aae-ad9c60ef659e)  
![Delete Employee Screenshot 2](https://github.com/user-attachments/assets/f290d02f-51e4-4933-bac3-cdae605e558a)

- **How it works:**
  - Reads the file and stores its data in a list of strings.
  - Iterates over the list and skips the employee with the specified ID.
  - Overwrites the file with the remaining employee data.

## File Handling Operations

1. **Read the File**
   - Reads rows of the file.
   - Iterates over the rows and stores data in a string (with attributes separated by commas).

2. **Save Employee Details**
   - Adds a new row to the file with the new employee.
   - If the header is null, it creates the header with attributes: `ID, Name, Age, Position, Salary, Email, Address`.

3. **Update Employee File**
   - Overwrites the file with the new employee data.

4. **Convert File to Object**
   - Converts a row in the file into an employee object with the specified details.

5. **Return Last Line of the File**
   - Returns the last row of the file to determine the last ID added.

## Employee Class

The `Employee` class contains basic **set** and **get** operations to update its attributes and also includes validation for input fields.

## Technologies Used

- **Python** for backend development.
- **File Handling** for CRUD operations.
- **Basic Input Validation** for employee details.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/user/Employee-Management-System.git
