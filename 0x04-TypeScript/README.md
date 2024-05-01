The ALX Project; Typescript
This project focus is on TypeScript, a programming language developed by Microsoft. It is a superset of JavaScript, which means that any valid JavaScript code is also valid TypeScript code. TypeScript extends JavaScript by adding static types to the language. These types provide a way to describe the shape of an object, providing better documentation, and allowing TypeScript to validate that your code is working correctly.

Follow the steps below to understand the project requirements and how to complete each task.

Task 0: Setting Up the Project

Copy the provided configuration files (package.json, .eslintrc.js, tsconfig.json, webpack.config.js) into the task_0 directory.

Write your TypeScript code in the main.ts file.

Task 1: Working with Interfaces and Classes

Create an interface named Student with the following attributes:
firstName (string)
lastName (string)
age (number)
location (string)
Create two students and store them in an array called studentsList.
Render a table using Vanilla JavaScript. Append a new row to the table for each student in the studentsList array. Each row should display the first name and location of the student.

Implement a Teacher class with the following attributes:

firstName and lastName (modifiable only during initialization)
fullTimeEmployee (boolean, always defined)
yearsOfExperience (optional number)
location (string, always defined)
Add the ability to add any attribute to the object without specifying the name.
Task 2: Extending Interfaces and Implementing Classes

Write an interface named Directors that extends the Teacher interface and requires an attribute named numberOfReports (number).

Implement a function printTeacher that takes firstName and lastName as arguments and returns a formatted string (e.g., "J. Doe").

Create a class StudentClass with the following features:

Constructor accepting firstName and lastName arguments.
Method workOnHomework that returns "Currently working".
Method displayName that returns the student's first name.
Task 3: Working with Interfaces, Types, and Libraries

Create a DirectorInterface with methods:

workFromHome() returning a string
getCoffeeBreak() returning a string
workDirectorTasks() returning a string
Create a TeacherInterface with methods:

workFromHome() returning a string
getCoffeeBreak() returning a string
workTeacherTasks() returning a string
Implement Director and Teacher classes that implement DirectorInterface and TeacherInterface respectively.

Implement a function createEmployee that returns either a Director or a Teacher instance based on the provided salary.

Write a function isDirector that checks if an employee is a Director.

Write a function executeWork that calls appropriate tasks based on the employee's type (Director or Teacher).

Task 4: Working with String Literal Types

Write a String literal type named Subjects allowing variables to have the value "Math" or "History" only.

Implement a function teachClass that takes todayClass as an argument and returns a string:

"Teaching Math" if todayClass is "Math".

"Teaching History" if todayClass is "History".

Task 5: Database Interaction and Namespace Usage

Create an interface.ts file with a RowID type (number) and a RowElement interface containing firstName (string), lastName (string), and optional age (number).

Write type declarations in an ambient file crud.d.ts for CRUD functions. Import RowID and RowElement from interface.ts.

In main.ts, use CRUD functions to manipulate data based on RowID and RowElement types.

Task 6: Working with Namespaces and Classes

Create a directory task_4 and copy the provided tsconfig.json and package.json into it.

In task_4/js/subjects/Teacher.ts, define a Teacher interface within the Subjects namespace with firstName and lastName attributes.

In task_4/js/subjects/Subject.ts, create a Subject class within the Subjects namespace with a teacher attribute implementing the Teacher interface. Implement a setTeacher method to set the teacher.

In task_4/js/subjects/Cpp.ts, extend the Teacher interface using declaration merging to add an optional experienceTeachingC attribute. Create a Cpp class extending Subject with methods getRequirements and getAvailableTeacher.

Repeat step 4 for React and Java classes with experienceTeachingReact and experienceTeachingJava attributes respectively.

Export constants cpp, java, and react representing instances of Cpp, Java, and React classes. Set the appropriate teachers and log the requirements and available teachers.

Task 7: Working with Interfaces and Functions

Create a directory task_5 and copy the provided tsconfig.json, package.json, and webpack.config.js into it.

In task_5/js/main.ts, create two interfaces MajorCredits and MinorCredits. Add a credits property and a unique brand property to each interface.

Implement functions sumMajorCredits and sumMinorCredits that take two arguments (subject1 and subject2) and return the sum of credits for major and minor subjects respectively.
