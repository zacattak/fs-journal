# A bit more CSharp and SQL
1. What does ***inheritance*** accomplish for us in C#?

  > In C# inheritance enables one class to inherit properties, members, and other members from another class. 

2. How does ***member inheritance*** work in C#? Does a `Class` inherit all members of the base `Class`?

  > Inheritance enables you to create new classes that reuse extend and modify the behavior of other classes. The class that does the inheriting is called the derived class, and the class that is inherited from is called the derived class. Derived classes are limited to one base class. Each derived class represents different "specializations" of the base class. Derived classes implicitly gain all of the members of a base class.

3. How does ***accessibility*** affect inheritance?

  > Accessibility refers to the visibility of base class members in regards to the corresponding derived class. For example, a private member would only be visible, and accessible, to derived classes that are nested within their base classes.

4. What is the difference between a `PRIMARY KEY` and a `FOREIGN KEY`

  >  A primary key is a unique identifier tied to each row in a table, while a foreign key represents a relationship between two tables.

5. What is an ***alias***?

  > An alias refers to an alternative or shorthand name given to a variable, function, class, or any other qualifying entity within the code.

6. Demonstrate how you would query a join statement that would get all of a doctors patients from the following collections:

  ```SQL
  CREATE TABLE doctors (
    id INT NOT NULL AUTO_INCREMENT,
    patientId INT NOT NULL,
    PRIMARY KEY (id)
  )

  CREATE TABLE patients (
    id INT NOT NULL AUTO_INCREMENT,
    doctorId INT NOT NULL,
    PRIMARY KEY (id)
  )

  CREATE TABLE patient_doctors (
    id INT NOT NULL AUTO_INCREMENT,
    doctorId INT NOT NULL,
    patientId INT NOT NULL,

    FOREIGN KEY (doctorId)
      REFERENCES doctors(id),
    FOREIGN KEY (patientId)
      REFERENCES patients(id),
  )

  SELECT 
  patient_doctor.*,
  patient.*,
  FROM patient_doctors patient_doctor
  JOIN patients patient
  ON doctor.patientId = patient.id


  ```

  > 
