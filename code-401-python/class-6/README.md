# What are Design Patterns

A design pattern is only a description or template for how to solve a problem!
### There is 3 major types of design patterns:


## There is 3 major types of design patterns:

### 1. Creational Patterns:

### Some Creational Patterns:

* #### Factory Method :  The factory pattern is used to replace class constructors, abstracting the process of object generation so that the type of the object instantiated can be determined at run-time.

* #### Singleton : The singleton pattern ensures that only one object of a particular class is ever created. All further references to objects of the singleton class refer to the same underlying instance.

* #### Abstract Factory : The abstract factory pattern is used to provide a client with a set of related or dependent objects. The “family” of objects created by the factory are determined at run-time.


# Dependency Injection
dependency injection is a technique whereby one object (or static method) supplies the dependencies of another object. A dependency is an object that can be used (a service).

dependency in programming means:
When class A uses some functionality of class B, then its said that class A has a dependency of class B.



### There are basically three types of dependency injection:

1. constructor injection: the dependencies are provided through a class constructor.
2. setter injection: the client exposes a setter method that the injector uses to inject the dependency.
3. interface injection: the dependency provides an injector method that will inject the dependency into any client passed to it

## Benefits of using dependency injection
1. Helps in Unit testing.
2. Boiler plate code is reduced, as initializing of dependencies is done by the injector component.
3. Extending the application becomes easier.
4. Helps to enable loose coupling, which is important in application programming.

## Disadvantages of dependency injection
1. It’s a bit complex to learn, and if overused can lead to management issues and other problems.
2. Many compile time errors are pushed to run-time.
3. Dependency injection frameworks are implemented with reflection or dynamic programming. This can hinder use of IDE automation, such as “find references”, “show call hierarchy” and safe refactoring.

## Why use Risk Analysis?
In any software, using risk analysis at the beginning of a project highlights the potential problem areas. After knowing about the risk areas, it helps the developers and managers to mitigate the risks. When a test plan has been created, risks involved in testing the product are to be taken into consideration along with the possibility of the damage they may cause to your software along with solutions.

The perspective of Risk Assessment
There are three perspectives of Risk Assessment:
- Effect

- Cause

- Likelihood

* * Effect – To assess risk by Effect. In case you identify a condition, event or action and try to determine its impact.

* * Cause – To assess risk by Cause is opposite of by Effect. Initialize scanning the problem and reach to the point that could be the most probable reason behind that.

* * Likelihood – To assess risk by Likelihood is to say that there is a probability that a requirement won’t be satisfied.




## References

https://www.freecodecamp.org/news/a-quick-intro-to-dependency-injection-what-it-is-and-when-to-use-it-7578c84fa88f/


https://datacadamia.com/code/design_pattern/injection#:~:text=Setter%20Injection%20is%20a%20Dependency,via%20setter%20methods%20after%20instantiation.

https://www.freecodecamp.org/news/a-quick-intro-to-dependency-injection-what-it-is-and-when-to-use-it-7578c84fa88f/

https://www.edureka.co/blog/risk-analysis-in-software-testing/#WhyuseRiskAnalysis?