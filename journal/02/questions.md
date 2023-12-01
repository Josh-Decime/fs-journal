# Intro to JavaScript
01. Which keywords are used to declare a variable in JavaScript?

    > var, let, const

02. What is the definition of a function?

    > It is a subprogram that is created to perform a specific task

03. What are the `SOLID` principles?

    > Single responsibility, Open-closed, Liskov Substitution, Interface Segregation, Dependency Inversion

04. Given this array: How could you remove the `pineapple`?

    ```js
    let fruit = ['apple', 'banana', 'pineapple', 'orange', 'strawberry']
    ```

    > let index = fruit.indexOf('pineapple'); {
        fruit.splice(index, 1)
        console.log(fruit)
    }

05. Given these two objects: How could you add each to the others friends arrays?

    ```js
    let you = {
        name: "You",
        hair: true,
        friends: []
    }
    let them = {
        name: "Them",
        hair: false,
        friends: []
    }
    ```

    > them.friends.push(you);
    you.friends.push(them);
    console.log(you.friends)
    console.log(them.friends)

06. Give an example of a JavaScript `Conditional`:

    > if, else, else if

07. What is the main difference between `parameters` and `arguments`?

    > a parameter does not have a concrete value but an argument is a value passed from function invocation

08. Instead of writing everything to the console, what is a better way to debug your code?

    > the debugger tool

09. What is the difference between a `primitive` value and a `reference` value?

    > primitives are predefined & reference values are created by the programmer

10. Demonstrate a loop that prints the numbers between -100 and 100?

    > for (let i = -100; i <= 100; i++){
    console.log(i)
