# reimagined-design-patterns

Give a summary description of Four design patterns that you choose from the following design patterns: **Adapter,  Builder, Composite, Decorator, Observer, Interpreter, State, Mediator, Memento, Prototype, Proxy**. In your summaries say:

- what kind of problem(s) you can solve with that pattern and when you use it, maybe with a short example
- how the pattern works, what the basic idea of the pattern is
- what the main advantage and what the the main disadvantage is of using this pattern
- Write a short summary for each of the four patterns, about half a page for each pattern (rather less than more). 

> Do not add diagrams, and do not try to give a complete description of the patterns as found in the books. Rather think of how you would explain the essential ideas of these patterns in a few sentences to a colleague while drinking coffee.

**Adapter pattern**

To inetract between two incompatible objects. Adpater class will be used as an intermediate between two objects to convert one format to another.

Example: Server does the operation in json format, but client pass the data in XML fomrat. In this case an adapter class can be used to convert from json to XML

Advantage: Reusablity. Need not to change existing implementation inorder to support new format.

Disadvantage: Increase in the overhead.

**Observer pattern**

If a state of an object is changed, it notifies all the dependends/subscribers automatically.

Example: If user subscibe any youtube channel, he will be notified if a new video is posted in the channel.

Advantage: 1) Subject only knows that observer implement Observer interface.Nothing more.
           2) There is no need to modify Subject to add or remove observers.

Disadvantage: If not correctly implemented, the Observer can add complexity and lead to inadvertent performance issues.

**Builder pattern**
This pattern used to create complex object step by step. 
Usually constructors are being used not initialize the object. But some of the constructor paramter may not be relevant for some objects. So class will become ugly if we introduce many paramters to the constructor. In builder pattern, to create an object, you execute a series of these steps on a builder object. The important part is that you don’t need to call all of the steps. You can call only those steps that are necessary for producing a particular configuration of an object.

Example: Consider the construction of home. Home is the final product that is to be returned as the output of the construction process. It will have many steps like basement construction, wall construction and so on roof construction

Advantage: 1) The parameters to the constructor are reduced 
           2) Object is always instantiated in a complete state

Disadvantage: 1)The number of lines of code increase at least to double.
              2)Requires creating a separate ConcreteBuilder for each different type of Product

