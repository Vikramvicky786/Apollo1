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

⭐