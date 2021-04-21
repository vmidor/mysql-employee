# mysql-employee
# Unit 12 MySQL Homework: Employee Tracker

Developers are often tasked with creating interfaces that make it easy for non-developers to view and interact with information stored in databases. Often these interfaces are known as **C**ontent **M**anagement **S**ystems. In this homework assignment, your challenge is to architect and build a solution for managing a company's employees using node, inquirer, and MySQL.

## Instructions

Design the following database schema containing three tables:

![Database Schema](assets/schema.png)
* **department**:

  * **id** - INT PRIMARY KEY
  * **name** - VARCHAR(30) to hold department name

* **role**:

  * **id** - INT PRIMARY KEY
  * **title** -  VARCHAR(30) to hold role title
  * **salary** -  DECIMAL to hold role salary
  * **department_id** -  INT to hold reference to department role belongs to

* **employee**:

  * **id** - INT PRIMARY KEY
  * **first_name** - VARCHAR(30) to hold employee first name
  * **last_name** - VARCHAR(30) to hold employee last name
  * **role_id** - INT to hold reference to role employee has
  * **manager_id** - INT to hold reference to another employee that manages the employee being Created. This field may be null if the employee has no manager

## User Story
  ```
As a business owner
I want to be able to view and manage the departments, roles, and employees in my company
So that I can organize and plan my business
```
![Employee Tracker](assets/employee-tracker.gif)
## Installation
```
npm i - to install all file in order for npm to work
npm i inquirer - to use inquirer (to interact with the user via command line)
npm init - to create a json file
npm i mysql - to connect to MySql database
npm console.table - to format tables
```

## Deployed video 
![video](https://drive.google.com/file/d/1MbaMxEERktQaN4wbaAV5GqbNOHrEE9vz/view)

