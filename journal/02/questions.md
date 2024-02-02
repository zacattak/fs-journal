# Intro to JavaScript
01. Which keywords are used to declare a variable in JavaScript?

    >Const is the keyword we have most commonly used in class, however var also declares a variable.

02. What is the definition of a function?

    > A function is a set of statements that perform a specified task or calculate a value.

03. What are the `SOLID` principles?

    > SOLID is an acronym that stands for a set of design principles. The acronym stands for single responsibility principle, open-closed principle, liskov substitution principle, interface segregation principle, and dependency inversion principle.

04. Given this array: How could you remove the `pineapple`?

    ```js
    let fruit = ['apple', 'banana', 'pineapple', 'orange', 'strawberry']
    ```

    > const newArray = array.filter(fruit => fruit !== 'pineapple')

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

    you.friends = [them];
    them.friends = [you];

06. Give an example of a JavaScript `Conditional`:

    if (5>4)
    then

07. What is the main difference between `parameters` and `arguments`?

    Parameters are variables that act as placeholders for a functions inputs or arguments. The arguments refer to the specific values that are assigned during the invocation of a function.

08. Instead of writing everything to the console, what is a better way to debug your code?

   Good debugging alternatives to writing everything to the console consist of employing the help of a debugger on your script as well as inspecting particular lines of code in your console and setting breakpoints to isolate parts of code.

09. What is the difference between a `primitive` value and a `reference` value?

    > Primitive types refer to data specifically defined and stored by the javascript language including number, string and object, whereas reference types refers to data stored by reference in the code.

10. Demonstrate a loop that prints the numbers between -100 and 100?

    for (let i = -100; i<100; i++){
    console.log(i);
    }
