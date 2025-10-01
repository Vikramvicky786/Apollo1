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