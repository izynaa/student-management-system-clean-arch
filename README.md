# Student Management System

## Introduction
This project has implemented all the crud operations in a simple way with H2 embedded database, custom exceptions and tests for controller class and service class.

## Features of this Project
- Save
- Show all
- Find by ID
- Find by Email
- Find by Index number
- Find between two dates of birth
- Update by ID
- Delete by ID
- Delete by Email

## Environment
- Eclipse IDE
- Java 11
- Spring
- Spring initializr
- H2 Embedded Database

## Operating Instructions
- Download source code and import into your code editor (Eclipse, IntelliJ..).
- The project is created with Maven, so you just need to import it to your IDE and build the project to resolve the dependencies
- If there are no errors, run program.
- Use [Postman](https://www.postman.com) to check app or use tests.

## Testing
### URL : http://localhost:8080/api/v1/student-ms/students + 
- ## POST METHOD
- ### /add
Add student with this in body: <br/>
{ <br/>
    "firstName": "Ognjen", <br/>
    "lastName": "Andjelic", <br/>
    "dateOfBirth": "1994-06-23", <br/>
    "email": "andjelicb.ognjen@gmail.com", <br/>
    "indexNumber": 101, <br/>
    "isOnBudget": true / false <br/>
}
- ## GET METHOD
- ### /all
List all students from DB.

- ### /find/{id}
Find student in DB by ID.

- ### /email/{email}
Find student in DB by Email.

- ### /index/{index}
Find student in DB by Index.

- ### /date-of-birth
Find students (list) between two dates of birth. <br/>
Put this as example parameters: <br/>
KEY: dob1 <br/>
VALUE: 1999-12-01 <br/>
KEY: dob2 <br/>
VALUE: 2004-10-12

- ## PUT METHOD
- ### /update/{id}
Update student with ID. <br/>
Add data in the body like saving student but you don't need to input all fields. <br/>
Input only fields that you want to change.

- ## DELETE METHOD
- ### /delete/{id}
Delete student with ID.

- ### /delete-with-email/{email}
Delete student with Email.

