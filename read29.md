# React Router

**React Router is a collection of navigational components that compose declaratively with your application.** Whether you want to have bookmarkable URLs for your web app or a composable way to navigate in React Native, React Router works wherever React is rendering--so take your pick! WebNative.

## The Router

We have three packages of React Router: 

- `react-router`: That package provides the core routing components and functions for the applications.
- `react-router-dom`: for browser components.
- `react-router-native`: for React Native components.

For browser based projects, there are two components:

- `<BrowserRouter>` : used when you have a server that will handle dynamic requests.(knows how to respond to any possible URI)
- `<HashRouter>`:  used for static websites (where the server can only respond to requests for files that it knows about).

## History

Each router creates a **history object**,to keep track of the current route and re-render the website whenever that changes.

## Rendering a Router

`<BrowserRouter>` which is a Router components expect to receive a single child element.

## Path

 where we pass the path prop in atring format that indecates the components or location

 ```javascript

 <Route exact path='/roster'/>

 ```

## How React Router Matches paths

Using the `path-to-regexp` package, It compiles the path string into a regular expression, which will be matched against the location’s pathname.

## What does the `<Route>` render

- `component`:  class component
- `render`:  function component
- `children`: this will always be rendered, regardless of whether the route’s path matches the current location.

