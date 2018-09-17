# Design-Principles

5 basic principles of object-oriented programming and design.

Classes are the building blocks of your java application. If these blocks are not strong, your building (i.e. application) is going to face the tough time in future. This essentially means that not so well-written can lead to very difficult situations when the application scope goes up or application faces certain design issues either in production or maintenance.

On the other hand, set of well designed and written classes can speed up the coding process by leaps and bounds, while reducing the number of bugs in comparison.

S.O.L.I.D Class Design Principles

Single Responsibility Principle - One class should have one and only responsibility
Open Closed Principle - Software components should be open for extension, but closed for modification
Liskov’s Substitution Principle - Derived types must be completely substitutable for their base types
Interface Segregation Principle - Clients should not be forced to implement unnecessary methods which they will not use"
Dependency Inversion Principle - "Depend on abstractions, not on concretions"

Single Responsibility Principle
"One class should have one and only one responsibility"
In other words, you should write, change and maintain a class for only one purpose. If it is model class then it should strictly represent only one actor/ entity. This will give you the flexibility to make changes in future without worrying the impacts of changes for another entity.
Similarly, If you are writing service/manager class then it should contain only that part of method calls and nothing else. Not even utility global functions related to module. Better separate them in another globally accessible class file. This will help in maintaining the class for that particular purpose, and you can decide the visibility of class to specific module only.


Revising !!!
Separate what changes from what Stays the Same!
Classes should be open for Extension, but closed for Modification!
Favor Composition over Inheritance
Program to an interface. Not an implementation
Strive for Loosely Coupled Designs
