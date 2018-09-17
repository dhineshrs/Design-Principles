# Design-Principles #

## 5 basic principles of object-oriented programming and design. ##


Classes are the building blocks of your java application. If these blocks are not strong, your building (i.e. application) is going to face the tough time in future. This essentially means that not so well-written can lead to very difficult situations when the application scope goes up or application faces certain design issues either in production or maintenance.

On the other hand, set of well designed and written classes can speed up the coding process by leaps and bounds, while reducing the number of bugs in comparison.

### S.O.L.I.D Class Design Principles ###

- Single Responsibility Principle - One class should have one and only responsibility
- Open Closed Principle - Software  - components should be open for extension, but closed for modification
- Liskov’s Substitution Principle  - Derived types must be completely substitutable for their base types
- Interface Segregation Principle  - Clients should not be forced to implement unnecessary methods which they will not use"
- Dependency Inversion Principle  - "Depend on abstractions, not on concretions"

### Single Responsibility Principle ###

"One class should have one and only one responsibility"

In other words, you should write, change and maintain a class for only one purpose. If it is model class then it should strictly represent only one actor/ entity. This will give you the flexibility to make changes in future without worrying the impacts of changes for another entity.

Similarly, If you are writing service/manager class then it should contain only that part of method calls and nothing else. Not even utility global functions related to module. Better separate them in another globally accessible class file. This will help in maintaining the class for that particular purpose, and you can decide the visibility of class to specific module only.

### Open Closed Principle ###

This is second important rule which you should keep in mind while designing your application. 
It says: "Software components should be open for extension, but closed for modification"

What does it mean?? It means that your classes should be designed such a way that whenever fellow developers wants to change the flow of control in specific conditions in application, all they need to extend your class and override some functions and that’s it.
If other developers are not able to design desired behavior due to constraints put by your class, then you should reconsider changing your class. I do not mean here that anybody can change the whole logic of your class, but he/she should be able to override the options provided by software in unharmful way permitted by software.

For example, if you take a look into any good framework like struts or spring, you will see that you can not change their core logic and request processing, BUT you modify the desired application flow just by extending some classes and plugin them in configuration files.

Revising !!!
- Separate what changes from what Stays the Same!
- Classes should be open for Extension, but closed for Modification!
- Favor Composition over Inheritance
- Program to an interface. Not an implementation
- Strive for Loosely Coupled Designs
