[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/2Itu1aHv)
# PBLJ5_Kapil-E18497-
Assignment: Java Programming Concepts
Part A: Autoboxing, Unboxing, and Sum Calculation
Objective: To understand the concepts of autoboxing and unboxing in Java and how they can be utilized to simplify the manipulation of primitive data types with wrapper classes.

Explanation: Autoboxing is the automatic conversion of a primitive type to its corresponding wrapper class. Unboxing is the reverse process, where an object of a wrapper class is automatically converted back to the corresponding primitive type.

In this part of the assignment, we will calculate the sum of a list of integers using both autoboxing and unboxing techniques. We will also demonstrate parsing strings into their respective wrapper classes.

Example Input:


String[] numberStrings = {"10", "20", "30", "40"};
List<Integer> integerList = new ArrayList<>();
for (String number : numberStrings) {
    integerList.add(Integer.parseInt(number));  // Parsing string to Integer
}
Example Output:


Sum of integers: 100
Part B: Serialization and Deserialization of a Student Object
Objective: To understand the concepts of serialization and deserialization in Java and how they are used to store and retrieve objects.

Explanation: Serialization is the process of converting an object into a byte stream to save it to a file, while deserialization is the reverse process of reconstructing the object from the byte stream.

In this part of the assignment, we will create a Student class, serialize it into a file, and then deserialize it back into an object.

Example Input:

Creating a Student object:


Student student = new Student("John Doe", 22, "Computer Science");
Serialization (writing the object to a file):


ObjectOutputStream out = new ObjectOutputStream(new FileOutputStream("student.ser"));
out.writeObject(student);
Deserialization (reading the object back):


ObjectInputStream in = new ObjectInputStream(new FileInputStream("student.ser"));
Student deserializedStudent = (Student) in.readObject();
Example Output:

Deserialized Student:
Student{name='John Doe', age=22, course='Computer Science'}
Part C: Menu-Based Application for Employee Management
Objective: To create a menu-based Java application that allows the addition and display of employee details, and stores this information in a file for persistence.

Explanation: This part demonstrates how to use a simple text-based menu to allow users to interact with a program. It involves creating an Employee class with details such as name, employee ID, designation, and salary. We will provide options to add an employee and display all employee details.

Menu Options:

Add an Employee: Gather employee details (name, ID, designation, salary) and store them in a file.
Display All Employees: Retrieve and display all stored employee details from the file.
Exit: Exit the program.
Example Input (Adding Employee):

Name: John Smith
Employee ID: 101
Designation: Software Developer
Salary: 75000
Example Output (After Adding Employee):


Employee added successfully!
Example Input (Display All Employees):


Employee ID: 101
Name: John Smith
Designation: Software Developer
Salary: 75000
