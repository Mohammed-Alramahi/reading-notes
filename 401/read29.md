# Advanced State with Reducers

## Review, Research, and Discussion

1- How can we ensure that an effect hook runs only once?

React has a built-in hook called useEffect. Hooks are used in function components. The Class component comparison to useEffect are the methods componentDidMount , componentDidUpdate .

2- Can useState() update more than one state variable at the same time?

You could merge the loading and data states into a single state object, then use setState only once, resulting in only one render. Note that, unlike setState in class components, useState's setState does not combine objects with existing state; instead, it completely changes the object.

3- Is useState() synchronous?

Both useState and setState are asynchronous operations. The useState and setState methods do not return promises, despite the fact that they are asynchronous. As a result, we can't utilize async/await to obtain the updated state values or attach a then handler to it.

### Terms

- State Hook: The state is an instance of React Component can be defined as an object of a set of observable properties that control the behavior of the component. In other words, the State of a component is an object that holds some information that may change over the lifetime of the component.

- Component Lifecycle: The component's lifecycle functions are run in a predictable sequence. In general, the lifecycle methods of React components may be divided into four phases: initialization, mounting, updating, and unmounting.

### Preparation Materials

How does useReducer work?
Like the useState Hook, useReducer is used to store and update states. The first parameter is a reducer function, while the second is the initial state.

One of the new Hooks included with React 16.8 is useReducer. It's a replacement for the useState Hook that aids in the management of complicated state logic in React apps. UseReducer, when paired with other Hooks like useContext, may be a decent alternative to Redux or MobX — and in some cases, it can even be a better solution.

For those who may be unfamiliar with Redux, we’ll explore this concept a bit further. There are three main building blocks in Redux:

- A store is an immutable object that contains the state data for an application.
- A reducer is a function that, when triggered by an action type, returns some state data.
- An action, which instructs the reducer on how to alter the state. It must have a type property, and it may also have a payload property.

Although useState is a Basic Hook for simple state transformation and useReducer is an Additional Hook for more complicated state logic, it's worth noting that useState utilizes useReducer internally. This means you can do anything you do with useState with useReducer.

It's vital to remember that no single Hook can address all of our difficulties while developing a React project. It's all about knowing where each Hook is most suited, how to use them, and how to combine different Hooks so that we can manage state in our app in a predictable way.