# Hooks

Hooks are a new addition in React 16.8. They let you use state and other React features without writing a class. Hooks are backwards-compatible. This page provides an overview of Hooks for experienced ## users. This is a fast-paced overview.

## 📌 State Hook

```javascript
//useState
import React, { useState } from 'react';

function Example() {
  // Declare a new state variable, which we'll call "count"
  const [count, setCount] = useState(0);

  return (
    <div>
      <p>You clicked {count} times</p>
      <button onClick={() => setCount(count + 1)}>
        Click me
      </button>
    </div>
  );
}
```

```javascript
class Example extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      count: 0
    };
  }

  render() {
    return (
      <div>
        <p>You clicked {this.state.count} times</p>
        <button onClick={() => this.setState({ count: this.state.count + 1 })}>
          Click me
        </button>
      </div>
    );
  }
}
```

- Its initial state is created in the initial render.
- Its state can be updated on the fly.
- React would remember the hook's state in future renders.
- React would provide you with the right state based on the calling order.
- React would know which fiber does this hook belong to.

## Terms:

*Composition* : is a natural pattern of the component model. It’s how we build components from other components, of varying complexity and specialization through props.

*Children/Child Components* : Children allow you to pass components as data to other components, just like any other prop you use.

*Hash Routing* : allows you to build one-page apps where the navigation is done by changing the hash, so the browser does not have to reload the page.

*Link Routing* : React-Router provides the and components, which allow you to navigate to different routes.