# nodejs-design-patterns
### Builder Pattern
A builder will use functions to set the class properties instead of arguments
Instead of passing parameters to class, we will use chained functions.
Suppose a class takes lot of parameters, its hard to find out what the parameters are representing.
### Command Pattern
- Its like when you want to use a CLI for building an object. 
- Every command is an encapsulated class
- Every command class will have a execute function.
- The execute function will execute some operations based on its class properties.
- All the commands are invoked with a switch statement in an another class `conductor`
- The conductor class gives us the flexibility to do other operations with the commands such as maintaining a history of commands etc
### Factory Pattern
Its like you use one class to call other clases based on argumets passed to the factory.
### Observer Pattern
- Its like an internal pub/sub service which can work with the async nature of 
nodejs.
- The object which will subscribe to an observer should have a notify or any similar function which the Observer will call when a subscribed event is trigged in the observer
### Proxy Pattern
- Imagine proxy is like an asssistant for an office COE.
- Instead of calling the COE directly you call the assistant, who will decide is it appropirate for the COE to do.
- In the same way, a proxy function will call another main function based on the rules mantioned in the proxy function
### Singleton Pattern
- Single instance of the object will be used in the entire application
- Like contexts in Reaact
- While exporting the class module, export it with the new keyword
### Strategy Pattern
- A function called `changeStrategy()` inside the class will decide the working of the class.
- Think about strategy in Passport.js which will behave based on strategy like Google or facebook
