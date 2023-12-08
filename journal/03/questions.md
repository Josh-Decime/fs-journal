# Application Architecture, MVC Design Pattern
01. What are the Pillars of Object Oriented Programming (`OOP`)?
  
  > Abstraction, encapsulation, inheritance, polymorphism
  Abstraction is the process to hide internal processes from the user, with classes that represent real world objects. 
  Encapsulation keeps code organized & separated, with classes that contain code which relates to a specific feature or subject.
  Inheritance is when one class inherits properties from another class, which makes it possible to reuse code to add new features.
  Polymorphism is about creating multiple methods that have the same name, but are implemented differently, which leads to more flexible systems that can be maintained easier.

02. How does `export` differ from `export default`?
  
  > I am getting conflicting information on what the difference is. In the article for the reading this week they only briefly gloss over export vs default export. The only difference they mentioned is that if you import using their method you will get an error unless you use export default. I looked it up on google for more information & google says the difference is that you can only export a single value per file with default exports. But in the reading they still exported several with one export. 

03. What is Encapsulation?
  
  > Encapsulation is where you pack data & functions into one component, it is also known as bundling, grouping or binding. The components can be a class, function or object.

04. What are some of the benefits of the `Proxy` object that we are using in our structure for applications?
  
  > You can work on the proxy object so you aren't changing the original object. Proxy objects allow us to log properties, validate, format & many other things.

05. What the difference between a `class` and an instance of a `class`?
  
  > The class is the blueprint & an instance of a class is the objects contained within it.

06. What is a computed Property?
  
  > A computed property is a property of an object that doesn't store a fixed value. It calculates its value when you access it. It uses a getter to perform that calculation. 

07. What is the purpose of the `MVC` pattern?
  
  > It separates the view from the controller and model so that what is being displayed is separate from the data & they can change without affecting each other.

08. What is the job of the `Controller` in the `MVC` Pattern?
  
  > The controller works with the user input & updates the view after changes have been made to the model.

09. What is the job of the `Service` in `MVC`?
  
  > The service contains the "business logic" in your application.

10. What is the job of the `Model` in `MVC`?
  
  > The model manages the data in the application
