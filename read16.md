# Event-Driven Programming in Node.js
Event-Driven Programming is a logical pattern that we can choose to confine our programming within to avoid issues of complexity and collision.
# EventEmitter
Node.js natively provides us with a useful module called `EventEmitter` that allows us to get started incorporating Event-Driven Programming in our project right away.
There are several modules published on npm such as `EventEmitter2` and `EventEmitter3` which promise a faster performance than the native EventEmitter.
# Removing Listeners
To remove event listeners in EventEmitter we can use the removeListener or removeAllListeners method. It’s important to note that in the EventEmitter that comes built-in with Node you must pass a reference to the exact function you wish to remove when using the removeListener method. This means wherever you wish to remove the event, you’ll need to make sure the function is able to be referenced from that place in your code. For this reason it is often best to name your event handling functions and declaring them before you register the event listener, as opposed to leaving them anonymous.
# Object Oriented Programming + Event-Driven Programming

The Object Oriented approach promotes the idea that all behavior of an individual unit (or object) be handled from code within that unit. Using this approach, applications are built with many different units that all speak to and interact with each other.