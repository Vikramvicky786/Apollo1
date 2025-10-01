# Java Practice Problems

This repository contains Java programs that solve basic practice problems using clean code, methods, and return types. 

⭐Question:
 Write a Java program to demonstrate Method Overriding where a parent class defines a method and multiple child classes provide their own implementation.

🔹 Explanation:
 👉 Method Overriding occurs when a subclass provides a specific implementation of a method already defined in its superclass.
 👉 It enables Runtime Polymorphism – meaning the method to be executed is determined at runtime, not compile-time.
 👉 In this program:
Animal is the parent class with sound().
Dog and Cat override the method with their own implementations.

🔹 Logic:
Define a parent class Animal with method sound().
Create child classes Dog and Cat that override sound().
Use parent references to point to child objects → runtime polymorphism in action.

🔹 Working:
Animal a1 = new Animal(); → Calls parent’s method.
Animal a2 = new Dog(); → Calls Dog’s overridden method.
Animal a3 = new Cat(); → Calls Cat’s overridden method.

🔹 Example Input & Output:
Input (in code):
Animal a1 = new Animal();
a1.sound();

Animal a2 = new Dog();
a2.sound();

Animal a3 = new Cat();
a3.sound();

Output:
Animals make sounds
Dog barks
Cat meows

⭐Question:
 Write a Java program to demonstrate Method Overloading by creating a calculator that can add both integers and doubles.

🔹 Explanation:
 👉 Method Overloading in Java allows multiple methods in the same class with the same name but different parameter types or counts.
 👉 Here, the class Calculator has two add() methods:
One that takes integers
One that takes doubles
 👉 Depending on the arguments passed, the correct version is executed.

🔹 Logic:
Create a class Calculator with an int result variable.
Define two add() methods (overloaded):
add(int a, int b) → adds integers.
add(double a, double b) → adds doubles.
Use getResult() as a getter method for integer results.
In the main method, call both versions of add() and print results.

🔹 Working:
 The compiler decides which add() method to execute based on argument types:
If both are integers → integer add() executes.
If both are doubles → double add() executes.

🔹 Example Input & Output:
Input (in code):
System.out.println("Int result: " + c.add(5, 10));
System.out.println("Double result: " + c.add(2.5, 3.5));

Output:
Int result: 15
Double result: 6.0

⭐ Question:
Write a Java program to design a simple calculator that can perform:
 1️⃣ Addition
 2️⃣ Subtraction
 3️⃣ Multiplication
 4️⃣ Division
The user should input two numbers and choose an operation.

📝 Explanation:
A calculator is one of the best beginner-friendly programs.
 Here, we’ll use a switch statement to decide which operation to perform based on user input.

⚙️ Logic:
Take two integer inputs from the user.
Display operation choices (Add, Subtract, Multiply, Divide).
Use a switch case to perform the selected operation.
Handle division by zero safely.
Print the final result.

🔄 Working:
User enters two numbers.
User selects an operator (1, 2, 3, or 4).
Program executes the respective case and prints result.

📊 Example Input & Output:
✅ Input:
 Choose operator: 1
 Enter first number: 20
 Enter second number: 15
✅ Output:
 Result is: 35

 ⭐ Question:
Write a Java program to find and print the duplicate elements present in an integer array.

📝 Explanation:
When working with arrays, sometimes the same element appears more than once.
 
⚙️ Logic:
Take an array of integers.
Use two nested loops:
Outer loop picks each element.
Inner loop checks it with the remaining elements.
If a match is found → Print that element as a duplicate.

🔄 Working:
Input Array → {6, 2, 8, 1, 4, 2, 7, 9, 5, 1, 7, 4}
Check each number against all the numbers after it.
Print only if duplicates are found.

📊 Example Input & Output:
✅ Input:
 {6, 2, 8, 1, 4, 2, 7, 9, 5, 1, 7, 4}
✅ Output:
Duplicate elements found:
2
1
7
4

⭐Question:
Write a Java program to generate a random number between 1 and 100 and display it.

📝 Explanation:
👉 The task is to create a random number in the range 1–100.
 👉 Java provides the Random class from java.util package.
 👉 random.nextInt(100) generates numbers from 0 to 99.
 👉 By adding +1, we shift the range to 1–100.

⚙️ Logic:
Import java.util.Random.
Create an object of Random.
Use nextInt(100) + 1 to generate the number.
Print the result.

📊 Example Run:
Output 1:
 Generated number is: 34
Output 2:
 Generated number is: 87
(💡 Each time the output changes because it’s random!)

