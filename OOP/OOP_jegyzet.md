# Object Oriented Programming

## Inheritance
- **GOAL: recyclable, modularized code**
- `extends` is a keyword
- Direct / Indirect parents
- Java only has single inheritance
- Every class extends Object
- Inheritance hierarchy
- Instance variable shadowing (override variables)
- Polymorphism (override methods)
- Interpreter finds overriden methods, uses new one
- Interpreter cannot access subclass method, if Object is called as its superclass, 
and method is only present in sub (you need casting)
- `super` is a reference variable, refers to direct superclass
- The Diamond problem

## Acces modifiers
- **GOAL: encapsulation, extra security layer, Principle of Least Privilege**
- `default` also called package-private, visible only inside package
- `public` visible to every other Class
- `protected` visible to package and all subclasses
- `private` visible only inside the same class  => getters and setters
- `final` cannot change, and cannot be overriden
- `static` only one instance is present above all Class instances, therefore can be called by the Class name
- [Check modifiers here](http://net-informations.com/java/basics/img/access-modifier.png)

## Interfaces
- **GOAL: Code safety, decouples Class and its users, Separation of Concerns**
- An Interface is a contract between the implementing Class and the outside world
- Blueprint for a class, methods and fields are not specified, they are abstract
- Given members must be overridden, implemented
- Leads to polymorphism

## Abstract Classes
- **GOAL: Provide complie time safety, contain general ideas, support inheritance**
- `abstract`  modifiers used in Class decleration, and abstract methods
- Instance of abstract Class cannot be created, only inherited from
