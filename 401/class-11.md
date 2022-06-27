# Code 401 - Class 11 - Event Driven Applications

## [Event Driven Programming](https://www.digitalocean.com/community/tutorials/nodejs-event-driven-programming)

### What native Node.js module allows us to get started with Event Driven Programming?

- [EventEmitter](https://nodejs.org/api/events.html#events_class_eventemitter)

### What is the value of Object Oriented Programming used in tandem with Event Driven Programming?

- This helps to maintain control of functionality as applications get more complex. By using even listeners (via EventEmitter) an object can "emit" events, and whichever objects are listening to those events can process them as needed. This keeps each object's behaviors contained entirely within itself.

### Consider your knowledge of Event Driven Programming in the Web Browser, now explain to a non-technical friend how Event Driven Programming might be useful on the backend using Node.js

- Event Driven Programming is useful on a back end server, because it allows additional objects to be added that can make use of functionality in existing objects without needing to "reach into" them to access that functionality. Instead, the new objects can include even listeners that can listen to the events being emitted by the existing objects. This allows for more control when adding objects to a back end.

[Back to Home](../README.md)
