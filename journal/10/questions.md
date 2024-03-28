# CSharp and SQL Fundamentals
01. What is the purpose of a `namespace`?

  > Namespaces generally organize and manage codebases and defines their scope and boundaries. One of the ways in which they do this includes defining identifiers that can be used without conflicting with similarly named identifiers outside of the namespace. 

02. What is the difference between a `class` and an `interface`?

  > A class can be thought of as a blueprint for creating objects with specific attributes and behaviors, whereas an interface can be thought of as a "contract" for classes that defines goals and abstract methods for classes to share without sharing a common "ancestor".

03. What is the method that returns an instance of a class, yet it has no return type?

  > I believe the method being referred to here is called "constructor".

05. In the Car example what is the access modifier of the `Start()` method?

  ```c#
  abstract class Car
  {
    public string Start()
    {

      return "Vroooom";

    }
  }
  ```

  > The "access modifier" in  the above section of code would be "public".

06. In the Car example what is `string` an indication of?

  > String is referring to a data type.

07. In the Car example what is `abstract` preventing?

  > It prevents the class from being instantiated directly, and instead serves as a template for other classes to inherit from.

08. In a SQL table, what is the difference between information in a row and information in a column?

  > A row, AKA record, represents a single "instance" or entry to the table, whereas a column or "field" represents a single attribute shared by all rows in the table.

09. Demonstrate the necessary SQL for creating a table called `characters` with the values `name, age, description` as strings, and an `int` id.

  > CREATE TABLE characters (
    id INT PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(255),
    age VARCHAR(50),
    description VARCHAR(255)
);

10. In SQL how can you query more than a single table? Provide an example.

  > You can query more than one table at a time by using the 'JOIN keyword', for example if two tables had the shared attribute of departmentId you could say something like "JOIN departments d ON e.DepartmentID = d.DepartmentID;" after specifying what properties to select for and where to select from.
