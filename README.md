

[𝟭.] 𝗦𝗶𝗻𝗴𝗹𝗲𝘁𝗼𝗻 𝗣𝗮𝘁𝘁𝗲𝗿𝗻
Ensure a class has only one instance and provide a global point of access to it.

Use it -
◾ When you need exactly one instance of a class => logger, configuration manager, thread pool etc.
◾ When the sole instance needs to be globally accessible throughout the application.

⚠
◾ Use sparingly to avoid global state issues. Makes testing difficult.
◾ May be considered an anti-pattern in some scenarios due to potential overuse and tight coupling.
◾ Consider dependency injection for increased flexibility and testability.

[𝟮.] 𝗙𝗮𝗰𝘁𝗼𝗿𝘆 𝗠𝗲𝘁𝗵𝗼𝗱
Define an interface (or abstract class) for creating an object, but let subclasses decide which class to instantiate.

Use it -
◾ When a class cannot anticipate the class of objects it must create.
◾ When you want to localize the knowledge of which concrete classes are used.
◾ To promote loose coupling between the creator and the concrete products.

[3.] Abstract Factory
Provide an interface for creating families of related or dependent objects without specifying their concrete classes.


[𝟰.] 𝗕𝘂𝗶𝗹𝗱𝗲𝗿 𝗣𝗮𝘁𝘁𝗲𝗿𝗻
Separate the construction of a complex object from its representation, allowing the same construction process to create various representations.

Use it -
◾ When the construction process of a complex object involves multiple steps or variations.
◾ When you want to create different representations of an object using the same construction process.

[𝟱.] 𝗣𝗿𝗼𝘁𝗼𝘁𝘆𝗽𝗲
Specify the kinds of objects to create using a prototypical instance and create new objects by copying this prototype.

Use it -
◾ When the cost of creating an object is expensive => complex initialization
◾ When you want to avoid subclasses of an object creator in the client application.
◾ When you need to create objects with a specific state or configuration.



<img width="975" height="1268" alt="image" src="https://github.com/user-attachments/assets/700e27e4-df35-4bd4-bb4d-dae9ea4c2cbb" />


# DESIGN-PRINCIPLES 
SOLID principles are foundational to writing clean, maintainable, and extensible code.

💡 What is SOLID?
 SOLID is an acronym for five key object-oriented design principles that help developers build robust and scalable software:

✅ S - Single Responsibility Principle
 A class should have one and only one reason to change, meaning it should have a single, well-defined responsibility.

✅ O - Open/Closed Principle
 Software entities should be open for extension but closed for modification. You can add new behavior without changing existing, tested code.

✅ L - Liskov Substitution Principle
 Subtypes must be substitutable for their base types without altering the correctness of the program. Inheritance should preserve behavior.

✅ I - Interface Segregation Principle
 Clients should not be forced to depend on interfaces they don’t use. Split large interfaces into smaller, more specific ones.

✅ D - Dependency Inversion Principle
 High-level modules should depend on abstractions, not concrete implementations. This promotes loose coupling and easier testing.


<img width="940" height="1410" alt="image" src="https://github.com/user-attachments/assets/23fab8de-8226-4e96-86b6-1f135b04bddb" />
