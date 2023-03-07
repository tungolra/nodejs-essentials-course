# Design Patters 

## Overview 
- Gang of Four: 
    - essentials: 
        - pattern name: describes porblem and solution in a few words
        - the problem: should be clearly stated and when pattern should be used
        - the solution: clearly diagrammed and documented 
        - consequences: must define trade-offs when using them 
    - 3 categories: 
        - creational 
        - structural 
        - behavioural 
- Anti-patterns: bad patterns to avoid 
    - modifying the prototype on an instance 
    - using sync execution after initializing the app 
    - callback chaos

## Ch 2: Creational Patterns 

- 2.1-3: The Singleton problem: creating multiple instances of one object 
    - refactoring by exporting instance itself or creating a Singleton class with getInstance() method
- ch 2.4-5: using Prototype pattern to create similar instances of object
- ch 2.6: Factory method: encapsulating constructors into a single module and creating a function that will create object for us; subclasses decide which class to instantiate 
- ch 2.7: Builder pattern fixes teloscopic constructor problem - a constructor with too many arguments 
## Ch 3: Structural Patterns 
- 3.1: The Adapter pattern 
    - take an object, keep its interface, adapt it to new environment or solution; adaptors make incompatible classes become compatible
    - adapting localstorage to nodejs
- 3.3: using a proxy to use an interface that delays instantiation of expensive object and control requests made to that object
- 3.5: The Composite pattern: organize objects in a way that treats leafs and branches uniformly
- 3.7: Decorator pattern: attach additional responsibilities to an object dynamically as alternative to subclassing for extending functionality

## Ch 4: Behavioural Patterns 
- Chain of responsibility pattern: chain together objects to handle a request; handler could pass request to next handler, each handler being able to return a result
    - avoids coupling the sender of a request with its receiver 