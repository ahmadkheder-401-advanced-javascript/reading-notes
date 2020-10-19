# React Hooks

**Five Important Rules for Hooks**

- Never call Hooks from inside a loop, condition or nested function
- Hooks should sit at the top-level of your component
- Only call Hooks from React functional components
- Never call a Hook from a regular function
- Hooks can call other Hooks

**useState:** is a React hook. Hooks make possible to use state and mutability inside function components. While you can't use hooks inside classes you can wrap your class component with a function one and use hooks from it. This is a great tool for migrating components from class to function form.


## React Hooks with Async-Await

```
We cannot use 'async' keyword with 'useEffect' callback method. It will result in race conditions.
```

## Terms

- state hook:Hooks are a new addition in React 16.8. They let you use state and other React features without writing a class.
- effect hook:By using this Hook, you tell React that your component needs to do something after render. React will remember the function you passed (we'll refer to it as our “effect”), and call it later after performing the DOM updates.
- useReducer: is one of a handful of React hooks that shipped in React 16.7. 0. It accepts a reducer function with the application initial state, returns the current application state, then dispatches a function.
