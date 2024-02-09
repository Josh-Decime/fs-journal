# CSharp and SQL Fundamentals
01. What is the purpose of a `namespace`?

  > it is how C# imports & exports. It is set up in the Globals.cs file

02. What is the difference between a `class` and an `interface`?

  > Class allows you to create & implement functionality, but interface only allows you to define the functionality. A class can only extend one other (abstract) class but can utilize several interfaces

03. What is the method that returns an instance of a class, yet it has no return type?

  > void has no return 

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

  > the access modifier for start is the keyword public

06. In the Car example what is `string` an indication of?

  > string is the value type

07. In the Car example what is `abstract` preventing?

  > abstract prevents you from using the class on its own. As Mick puts it "abstract is a class you can never instantiate"

08. In a SQL table, what is the difference between information in a row and information in a column?

  > the row is information contained by a single entity while the column is information that all entities share

09. Demonstrate the necessary SQL for creating a table called `characters` with the values `name, age, description` as strings, and an `int` id.

  > CREATE TABLE characters(
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(30) NOT NULL,
    age VARCHAR(20) NOT NULL,
    description VARCHAR(3000) NOT NULL
  )

10. In SQL how can you query more than a single table? Provide an example.

  > you can query multiple tables using a joint operation. To populate the creator we join the account table to our recipe table using the creator id.
