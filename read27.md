# _

## setState

setState() is the only legitimate way to update state after the initial state setup.

## State and Lifecycle

When `<Clock />`is passed to `ReactDOM.render()` , React calls the constructor of the Clock component. Since Clock needs to display the current time, it initializes this.state with an object including the current time. ... When the Clock output is inserted in the DOM, React calls the componentDidMount() lifecycle method.

## Props

“Props” is a special keyword in React, which stands for properties and is being used for passing data from one component to another. But the important part here is that data with props are being passed in a uni-directional flow.

## Term

- BDD: Behaviour-Driven Development (BDD) is a collaborative approach to software development that bridges the communication gap between business and IT.
- Acceptance Tests: testing React and the behavior of the app, not individual components. based off inspecting the DOM.
- mounting:is the process of outputting the virtual representation of a component into the final UI representation 
- build: the compiling of all the files in a project to be able to go to production