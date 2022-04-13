
1. What are the types of design patterns in java?
    
    There are 23 design patterns that can be classified into three categories: Creational, Structural and Behavioral patterns.
    
    **Creational Patterns**
        
        These design patterns provide a way to create objects while hiding the creation logic, rather than instantiating objects directly using new operator. This gives program more flexibility in deciding which objects need to be created for a given use case.
        
        - [Singleton Pattern](https://www.journaldev.com/1827/java-design-patterns-example-tutorial#singleton-pattern)
        - [Factory Pattern](https://www.journaldev.com/1827/java-design-patterns-example-tutorial#factory-pattern)
        - [Abstract Factory Pattern](https://www.journaldev.com/1827/java-design-patterns-example-tutorial#abstract-factory-pattern)
        - [Builder Pattern](https://www.journaldev.com/1827/java-design-patterns-example-tutorial#builder-pattern)
        - [Prototype Pattern](https://www.journaldev.com/1827/java-design-patterns-example-tutorial#prototype-pattern)
    **Structural Patterns**
        
        These design patterns concern class and object composition. Concept of inheritance is used to compose interfaces and define ways to compose objects to obtain new functionalities.
        
        - [Adapter Pattern](https://www.journaldev.com/1827/java-design-patterns-example-tutorial#adapter-pattern)
        - [Composite Pattern](https://www.journaldev.com/1827/java-design-patterns-example-tutorial#composite-pattern)
        - [Proxy Pattern](https://www.journaldev.com/1827/java-design-patterns-example-tutorial#proxy-pattern)
        - [Flyweight Pattern](https://www.journaldev.com/1827/java-design-patterns-example-tutorial#flyweight-pattern)
        - [Facade Pattern](https://www.journaldev.com/1827/java-design-patterns-example-tutorial#facade-pattern)
        - [Bridge Pattern](https://www.journaldev.com/1827/java-design-patterns-example-tutorial#bridge-pattern)
        - [Decorator Pattern](https://www.journaldev.com/1827/java-design-patterns-example-tutorial#decorator-pattern)
    **Behavioral Patterns**
        
        These design patterns are specifically concerned with communication between objects.
        
        - [Template Method Pattern](https://www.journaldev.com/1827/java-design-patterns-example-tutorial#template-method-pattern)
        - [Mediator Pattern](https://www.journaldev.com/1827/java-design-patterns-example-tutorial#mediator-pattern)
        - [Chain of Responsibility Pattern](https://www.journaldev.com/1827/java-design-patterns-example-tutorial#chain-of-responsibility-pattern)
        - [Observer Pattern](https://www.journaldev.com/1827/java-design-patterns-example-tutorial#observer-pattern)
        - [Strategy Pattern](https://www.journaldev.com/1827/java-design-patterns-example-tutorial#strategy-pattern)
        - [Command Pattern](https://www.journaldev.com/1827/java-design-patterns-example-tutorial#command-pattern)
        - [State Pattern](https://www.journaldev.com/1827/java-design-patterns-example-tutorial#state-pattern)
        - [Visitor Pattern](https://www.journaldev.com/1827/java-design-patterns-example-tutorial#visitor-pattern)
        - [Interpreter Pattern](https://www.journaldev.com/1827/java-design-patterns-example-tutorial#interpreter-pattern)
        - [Iterator Pattern](https://www.journaldev.com/1827/java-design-patterns-example-tutorial#iterator-pattern)
        - [Memento Pattern](https://www.journaldev.com/1827/java-design-patterns-example-tutorial#memento-pattern)
2. What are the SOLID Principles?
    
    *SOLID* is an acronym for the first five object-oriented design (OOD) principles by Robert C. Martin (also known as [Uncle Bob](http://en.wikipedia.org/wiki/Robert_Cecil_Martin)).
    
    These principles establish practices that lend to developing software with considerations for maintaining and extending as the project grows. Adopting these practices can also contribute to avoiding code smells, refactoring code, and Agile or Adaptive software development.
    
    SOLID stands for:
    
    - **[S** - Single-responsiblity Principle](https://www.digitalocean.com/community/conceptual_articles/s-o-l-i-d-the-first-five-principles-of-object-oriented-design#single-responsibility-principle)
        
        A class should have one and only one reason to change, meaning that a class should have only one job.
        
    - **[O** - Open-closed Principle](https://www.digitalocean.com/community/conceptual_articles/s-o-l-i-d-the-first-five-principles-of-object-oriented-design#open-closed-principle)
        
        Objects or entities should be open for extension but closed for modification.
        
    - **[L** - Liskov Substitution Principle](https://www.digitalocean.com/community/conceptual_articles/s-o-l-i-d-the-first-five-principles-of-object-oriented-design#liskov-substitution-principle)
        
        Let q(x) be a property provable about objects of x of type T. Then q(y) should be provable for objects y of type S where S is a subtype of T.
        
    - **[I** - Interface Segregation Principle](https://www.digitalocean.com/community/conceptual_articles/s-o-l-i-d-the-first-five-principles-of-object-oriented-design#interface-segregation-principle)
        
        A client should never be forced to implement an interface that it doesn’t use, or clients shouldn’t be forced to depend on methods they do not use.
        
    - **[D** - Dependency Inversion Principle](https://www.digitalocean.com/community/conceptual_articles/s-o-l-i-d-the-first-five-principles-of-object-oriented-design#dependency-inversion-principle)
        
        Entities must depend on abstractions, not on concretions. It states that the high-level module must not depend on the low-level module, but they should depend on abstractions.
        
3. How can you achieve thread-safe singleton patterns in java?
    
    A lock must be obtained in case two or more threads call getHelper() simultaneously, otherwise, there may be problems: Both threads may try to create the object at the same time, leading to two objects. One thread may end up getting a reference to an incompletely initialized object.
    
4. What do you understand by the Open-Closed Principle(OCP)?
    
    The Open-Closed principle states that software entities should be *open for extension but closed for modification. This means that entities such as classes and modules should NOT be modified if they are already well defined, but they should allow other entities to inherit its properties or compose that entity within themselves. It is also about designing components where you wouldn’t need to modify them when you extend their functionality.