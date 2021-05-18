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

