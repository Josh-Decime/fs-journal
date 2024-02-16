# A bit more CSharp and SQL
1. What does ***inheritance*** accomplish for us in C#?

  > It allows us to inherit properties from another class which promotes code re-use & organization. This way we can add in or override existing functionality.

2. How does ***member inheritance*** work in C#? Does a `Class` inherit all members of the base `Class`?

  > Yes, it inherits all members of the base class, more or less. Some members might not be accessible because of their accessibility.

3. How does ***accessibility*** affect inheritance?

  > It determines which members of a base class can be inherited & accessed. This is private, public, internal, etc.

4. What is the difference between a `PRIMARY KEY` and a `FOREIGN KEY`

  > Primary key identifies each record of the table, while foreign key establishes a relationship with another table. This is used to join tables.

5. What is an ***alias***?

  > an alias is an alternate name. It set with AS. For example, when you make a COUNT you can say AS commentCount & it will be called commentCount in the table

6. Demonstrate how you would query a join statement that would get all of a doctors patients from the following collections:

  ```SQL
  CREATE TABLE doctors (
    id INT NOT NULL AUTO_INCREMENT,
    -- CODE OMITTED
    PRIMARY KEY (id)
  )

  CREATE TABLE patients (
    id INT NOT NULL AUTO_INCREMENT,
    -- CODE OMITTED
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

  ```

  > SELECT 
  patients.*
  FROM patients
  JOIN patients_doctors ON patients.id = patient_doctors.patientId
  JOIN doctors ON patient_doctors.doctorId = doctors.id
  WHERE doctors.id = @doctor_id:

