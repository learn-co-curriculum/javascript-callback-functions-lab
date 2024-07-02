# Lab - Callback Functions

## Overview

This lab will further help you understand the concepts surrounding Callback Functions.

Flatapets, a pet adoption center, wants to use callback functions to optimize the code for their website that allows its users to view details for pets that are available for adoption. You will need to use your knowledge of Callback Functions to complete this lab.

## Tools and Resources

It is recommended that you use the Visual Studio Code (VSCode) IDE for this lab.

Useful considerations and terminology:

**Function**: A special block of code that contains a set of statements that performs a task or calculates a value. A function can be called / invoked to execute its code.

**Callback Function**: A function that is passed in as an argument to another function and called / invoked within the other function.

Here are some resources from the [MDN Web Docs](https://developer.mozilla.org/en-US/) website that will provide you with additional knowledge about functions and callback functions:
- MDN
  - [Functions](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Functions)
  - [Callback function](https://developer.mozilla.org/en-US/docs/Glossary/Callback_function)

## Instructions

In this lab, you will practice using a callback function to optimize your code and make it more concise and readable.

**Fork and clone** this lab into your local environment. Navigate into its
directory in the terminal, then run `code .` to open the files in Visual Studio
Code.

Then, open the `index.html` file on your browser to run the application.

Write your code in the `index.js` file. There is some starter code provided in `index.js`.

These are your tasks:

1. `getPetDetails(petName, getPetMessage)`: Create a `function` named `getPetDetails` that has 2 parameters. The first parameter is named `petName` and its value should be a `string` with a pet’s name when the correct value is passed as an argument into the `getPetDetails()` function. The second parameter is named `getPetMessage` and its value should be a `function` when the correct value is passed as an argument into the `getPetDetails()` function. When the `getPetDetails()` function is called, the following actions should take place:
    - An `object` is created and stored into a variable named `pet`. The `object` contains a key of `name` whose value is set to the value of the `petName` parameter.
    - If the pet’s name is `"Fido"`, a key of `description` whose value is set to `"a dog that wants to be your best friend!"` is added to the `object` referenced by the variable named `pet`.
    - If the pet’s name is `"Kitty"`, a key of `description` whose value is set to `"a cat that wants to be your cute baby kitten!"` is added to the `object` referenced by the variable named `pet`.
    - If the pet’s name is `"Hammy"`, a key of `description` whose value is set to `"a hamster that is so tiny and cute!"` is added to the `object` referenced by the variable named `pet`.
    - If the pet’s name is `"Polly"`, a key of `description` whose value is set to `"a parrot. Polly wants a cracker!"` is added to the `object` referenced by the variable named `pet`.
    - If the pet’s name is `"Angel"`, a key of `description` whose value is set to `"a horse that begs politely, like an angel, for you to adopt it."` is added to the `object` referenced by the variable named `pet`.
    - If the pet’s name is `"Fluffy"`, a key of `description` whose value is set to `"a guinea pig that is so soft and fluffy!"` is added to the `object` referenced by the variable named `pet`.
    - If the pet’s name is `"Goldie"`, a key of `description` whose value is set to `"a goldfish that lives under the sea and looks forward to sea you soon."` is added to the `object` referenced by the variable named `pet`.
    - The `function` referenced by the `getPetMessage` parameter is called and its `return` value is returned from the `getPetDetails()` function.
      - For example: If the `return` value of `getPetMessage()` is `"Good night!"`, the `getPetDetails()` function should return `"Good night!"` as well.
2. `petMessage`: Call the `getPetDetails()` function and store its `return` value into a variable named `petMessage`. When calling the `getPetDetails()` function, the following 2 arguments should be passed into the `getPetDetails()` function:
    - The first argument passed into the `getPetDetails()` function is the value of the first pet name from the array stored in the `petNames` variable.
    - The second argument passed into the `getPetDetails()` function is an anonymous `function` that has one parameter named `pet` whose value should be an `object` that contains the following keys: `name` and `description`, when the correct value is passed as an argument into the anonymous function. When the anonymous function is called, a `string` in the following format is returned from the anonymous function: `"[name] is [description]"` — where `[name]` should be replaced with the pet’s name, and `[description]` should be replaced with the pet’s description.

## Submission and Grading Criteria

When you’re done with this lab, remember to commit and push your changes to GitHub, then submit your work to Canvas using CodeGrade.