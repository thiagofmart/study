# Design Patterns OverView
Design patterns are guidelines for solving repetitive problems.

Software design pattern is a general, reusable solution to a commonly ocurring problem within a given context in software design

---
## Creational Patterns
Category that focus on the process of object creation. They Provide a way to encapsulate the instantiation of objects, making it easier to manage object creation, maintain code modularity, and control the complexity of the system.

### Factory Method
This pattern defines an interface for creating an object, but lets subclasses decide which class to instantiate. Factory Method lets a class defer instantiation to subclasses, promotingloose coupling and extensibility.
### Abstract Factory
This pattern provides an interface for creating families of related or dependent objects without specifying their concrete classes. It is particularly useful when the system needs to work with multiple families of products or when you want to provide a library of products without exposing their implementation details
### Builder
This pattern separates the construction of a complex object from its representation, allowing the same construction process to create different representations. The builder pattern is useful when dealing with objects that have many optional or required parts, and when the object creation process needs to be more flexible or guided
### Prototype
This pattern specifies the kind of objects to create using a prototypical instance and creates new objects by copying this prototype. The Prototype pattern is especially useful when object creation is expensive or when a system needs to create objects dynamically at runtime.
### Singleton
This Pattern ensures that a class has only one instance and provides a global point of access to that instance. It is useful when you want to control access to a shared resource, such as a database connection or a configuration object

---
## Structural Patterns
Category that focus on the composition of classes and objects to create larger, more complex structures. These patterns help to ensure that the system is easy to maintain, scalable, and flexible by facilitating the organization of code and relationship between objects.

### Adapter
This pattern allows the interface of an existing class to be used as another interface, effectively enabling two incompatible interfaces to work together. It is useful when you want to integrate a new component with an existing system that has a different interface
### Bridge
This pattern decouples an abstraction from its implementation, enabling both to vary independently. It is particularly useful when you want to avoid a permanent binding between an abstraction and its implementation, or when the implementation can be selected or switched at runtime.
### Composite
This pattern allows you to compose objects into tree structures to represent part-whole hierarchies. Composite enables clients to treat individual objects and compositions of objects uniformly. It is useful when you want to manipulate a hierarchy of objects that share a common interface.
### Decorator
This pattern attaches additional responsibillities to an object dynamically without affecting other instances of the same class. Decorator provides a flexible alternative to subclassing for extending functionality. It is useful when you want to add new features to an object without modifying its structure or when you want to apply specific behavior to individual objects without affecting others.
### Facade
This pattern provides a unified interface to a set of interfaces in a subsystem making it easier to use and understand. Facade defines a higher-level interface that makes the subsystem or when you want to provide a clear, easy-to-use entry point for clients.
### Flyweight
This pattern uses sharing to support a large number of fine-grained objects efficiently. Flyweight minmizes memory usage by sharing as much data as possible with other similar objects. It is particularly useful when a system has many instances of a class that can share parts of their state.
### Proxy
This pattern provides a placeholder for another object to control access to it. Proxy can be used for various purposes, such as enforcing security restrictions, caching, or delaying the creation of expensive objects until they are actually needed. It is useful when you want to manage access to a resource or when you need a local representation of a remote object.

---
## Behavioral Patterns
Category that focus on the comunication and interaction between objects. These patteerns define how objects collaborate, delegate responsibilities, and share information, making it easier to manage the behavior and relationships within a system.

### Chain of Responsibility
This pattern creates a chain of receiver objects for a request. The request is passed along the chain until an object handles it. This pattern helps to decouple the sender and receiver of a request, allowing for dynamic addition or removal of handlers in the chain.
### Command
This pattern encapsulates a request as an object, allowing you to parameterize clients with different requests, queue or log requests, and support undoable operations. Command enables a separation of concerns between the object that issues a request and the object that executes it.
### Interpreter
This pattern defines a representation for a language's grammar and provides an interpreter to evaluate expressions in the language. It is useful when you need to design a system that processes a specific language or when you want to build a custom scripting language for your application.
### Iterator
This pattern provides a way to access the elements of an aggregate object sequentially without exponsing its underlying representation. Iterator enables you to traverse a collection of objects without depending on their specific implementation.
### Mediator
This pattern defines an objects that encapsulates how a set of objects interact, promoting loose coupling by keeping objects from referring to each other explicitly. Mediator helps to simplify the communication and dependencies between a group of related objects.
### Memento
This pattern captures and externalizes an object's internal state, allowing the object to be restored to this state later. Memento enables you to implement undo and rollback functionality, or save an object's state for later use without violating encapsulation.
### Observer
This pattern defines a one-to-many dependency between objects, so that when one object changes state, all its dependets are notified and updated automatically. Observer is useful when you want to create a system where the state of one object affects the state of other objects, such aas in a GUI framework or a data-driven application.
### State
This pattern allows an object to alter its behavior when its internal state changes. The object appears to change its class as its state changes. State is useful when an object's behavior depends on its state, and you want to simplify the implementation by separating state-specifc behaviors into different classess
### Strategy
This pattern defines a famil of algorithms, encapsulates each one, and makes them interchangeable. Strategy enables an algorithm's behavior to be selected at runtime, allowing for easy extension or replacement of algorithms without modifying the client code.
### Template Method
This pattern defines the skeleton of an algorithm in an operation, deferring some steps to subclasses. Template Method lets subclasses redefine certain steps of an algorithm without changing the algorithm's structure. It is useful when you want to provide a common structure for an algorithm while allowing for variations in specific steps.
### Visitor
This pattern represents an operation to be performed on elements of an object structure whitout cchanging the classes on which it operates. Visitor enables you to add new operations to existing classes without modifying their source code, making it especially useful for working with complex, heterogeneous data structures.
