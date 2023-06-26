# ASP-Project-HMS
Hospital Management System, ASP and VB , Database Sql Server 
# Database Schema

This repository contains the SQL code for creating the following tables in a database:

- `Department`
- `Nurse`
- `diseases`
- `doctors`
- `drugs`
- `employees`
- `patient`
- `rooms`
- `users`

## Instructions

To create these tables in your own database, you can copy and paste the SQL code into a query tool such as MySQL Workbench or phpMyAdmin and execute the queries. 

Note that the tables are created using the `InnoDB` engine and the `utf8mb4` character set.

## Table Descriptions

### Department

This table stores information about departments in a hospital.

| Column Name   | Data Type | Description                        |
|---------------|-----------|------------------------------------|
| DepartmentID  | tinyint   | ID of the department               |
| DepartmentName| varchar   | Name of the department             |
| DepartmentHead| varchar   | Name of the department head        |
| ContactNumber | varchar   | Contact number of the department   |
| Email         | varchar   | Email address of the department    |
| CreatedDate   | varchar   | Date when the department was added |

### Nurse

This table stores information about nurses in a hospital.

| Column Name   | Data Type | Description                        |
|---------------|-----------|------------------------------------|
| NurseID       | tinyint   | ID of the nurse                     |
| FirstName     | varchar   | First name of the nurse             |
| LastName      | varchar   | Last name of the nurse              |
| DateOfBirth   | varchar   | Date of birth of the nurse           |
| Gender        | varchar   | Gender of the nurse                  |
| ContactNumber | varchar   | Contact number of the nurse          |
| Email         | varchar   | Email address of the nurse           |
| Address       | varchar   | Address of the nurse                 |
| DateOfJoining | varchar   | Date when the nurse joined the hospital |
| ShiftStartTime| varchar   | Start time of the nurse's shift        |
| ShiftEndTime  | varchar   | End time of the nurse's shift          |
| Department    | varchar   | Department where the nurse works     |

### diseases

This table stores information about diseases.

| Column Name   | Data Type | Description                        |
|---------------|-----------|------------------------------------|
| Id            | tinyint   | ID of the disease                  |
| Name          | varchar   | Name of the disease                |
| RegDate       | varchar   | Date when the disease was registered |

### doctors

This table stores information about doctors.

| Column Name   | Data Type | Description                        |
|---------------|-----------|------------------------------------|
| id            | tinyint   | ID of the doctor                   |
| name          | varchar   | Name of the doctor                 |
| tellno        | int       | Telephone number of the doctor     |
| address       | varchar   | Address of the doctor              |
| email         | varchar   | Email address of the doctor        |
| gender        | varchar   | Gender of the doctor               |
| specialty     | varchar   | Specialty of the doctor            |
| created_at    | varchar   | Date when the doctor was added     |
| updated_at    | varchar   | Date when the doctor was updated   |

### drugs

This table stores information about drugs.

| Column Name   | Data Type | Description                        |
|---------------|-----------|------------------------------------|
| id            | tinyint   | ID of the drug                     |
| name          | varchar   | Name of the drug                   |
| issue_date    | varchar   | Date when the drug was issued      |
| expire_date   | varchar   | Date when the drug will expire     |
| country       | varchar   | Country where the drug was made    |
| qty           | tinyint   | Quantity of the drug               |
| price         | decimal   | Price of the drug                  |
| created_at    | varchar   | Date when the drug was added       |
| updated_at    | varchar   | Date when the drug was updated     |

### employees

This table stores information about employees.

| Column Name   | Data Type | Description                        |
|---------------|-----------|------------------------------------|
| Id            | varchar   | ID of the employee                 |
| Name          | varchar   | Name of the employee               |
| Tell          | varchar   | Telephone number of the employee   |
| Address       | varchar   | Address of the employee            |
| Age           | varchar   | Age of the employee                |
| Gender        | varchar   | Gender of the employee             |
| Jobtitle      | varchar   | Job title of the employee          |
| Salary        | varchar   | Salary of the employee             |
| RegDate       | varchar   | Date when the employee was registered |

### patient

This table stores information about patients.

| Column Name   | Data Type | Description                        |
|---------------|-----------|------------------------------------|
|id            | varchar   | ID of the patient                  |
| name          | varchar   | Name of the patient                |
| tellno        | varchar   | Telephone number of the patient    |
| address       | varchar   | Address of the patient             |
| Age           | varchar   | Age of the patient                 |
| gender        | varchar   | Gender of the patient              |
| Reg_fee       | varchar   | Registration fee of the patient    |
| created_at    | varchar   | Date when the patient was added    |

### rooms

This table stores information about rooms in a hospital.

| Column Name   | Data Type | Description                        |
|---------------|-----------|------------------------------------|
| id            | tinyint   | ID of the room                     |
| room_no       | varchar   | Room number                         |
| room_type     | varchar   | Type of the room                    |
| status        | varchar   | Status of the room                  |
| created_at    | varchar   | Date when the room was added        |
| updated_at    | varchar   | Date when the room was updated      |

### users

This table stores information about users of a system.

| Column Name   | Data Type | Description                        |
|---------------|-----------|------------------------------------|
| id            | tinyint   | ID of the user                     |
| name          | varchar   | Name of the user                   |
| username      | varchar   | Username of the user               |
| role          | varchar   | Role of the user                   |
| password      | mediumint | Password of the user               |
| created_at    | varchar   | Date when the user was added        |
| updated_at    | varchar   | Date when the user was updated      |
