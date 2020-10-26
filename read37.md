
##  Combined Reducers

combineReducers takes an object full of slice reducer functions, and creates a function that outputs a corresponding state object with the same keys. ... It's generally not a good practice to actually include words like "reducer" in your state key names - the keys should simply reflect the domain or type of data they hold.

## Terms

- immutable state:  state that cannot be modified after it is created. 
- time travel in redux: Time travel is the ability to move back and forth among the previous states of an application and view the results in real time. With Redux, given a specific state and a specific action, the next state of the application is always exactly the same. Redux is a predictable state container and it easy to implement time travel with it.

- action creator: is merely a function that returns an action object. Redux includes a utility function called bindActionCreators for binding one or more action creators to the store's dispatch() function.
- reducer:  a function that determines changes to an application's state. It uses the action it receives to determine this change. ... Redux relies heavily on reducer functions that take the previous state and an action in order to execute the next state. We're going to focus squarely on reducers is in this post

- dispatch:  a function of the Redux store. You call store. dispatch to dispatch an action. This is the only way to trigger a state change. ... connect can accept an argument called mapDispatchToProps , which lets you create functions that dispatch when called, and pass those functions as props to your component