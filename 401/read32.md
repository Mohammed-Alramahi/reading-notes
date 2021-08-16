# Context API - Behaviors

## Review, Research, and Discussion

### When you have multiple contexts, what component type should you use (class/function) and why?

  **The difference is pretty obvious. Class components are ES6 classes and Functional Components are functions. The only constraint for a functional component is to accept props as an argument and return valid JSX.**

### What are some good use cases for using the Context API for global state?

  - Stripe : Stripe is one of the most successful and best known API-driven businesses.
  - Google : Google is one of the most successful and best known API-driven businesses.
  
    Instead of being restricted to local states on views, you may now exchange data on a single central component and distribute it to its inner components (children, grandchildren and so forth). The centralized state is referred to as the store, and it may be distributed via the Context. Context and Provider Consumer 2- Data propagation and re-rendering: when this centralized global state (store) changes, it causes all of the children components (your whole application) to re-render, resulting in new data being displayed in the UI. A set in the middle 3- If you've dealt with react before, you've undoubtedly experienced the difficulty of passing properties around your project.

- How can you best test context?

Making our tests uninformed of Context's existence and avoiding mocks is the best approach to test it. We want to test our components in the same way that developers would (behavioral testing) and in the same way that they'd run in our apps (integration testing).

## Document the following Vocabulary Terms

- **context** is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language.

- **useContext()** hook is used to create data that can be accessed throughout the component hierarchy without passing the props down manually to each level. Context defined will be available to all the child components without including “props”.

- **static context**: If you are using the experimental public class fields syntax, you can use a static class field to initialize your contextType.

## Preparation Materials

### Context api

Context allows you to transmit data down the component tree without having to explicitly supply props at each level. Props are used to transfer data top-down (parent to child) in a normal React application, however this might be inconvenient for certain sorts of props (e.g. locale preference, UI theme).

Before You Use Context Context is primarily used when some data needs to be accessible by many components at different nesting levels. Apply it sparingly because it makes component reuse more difficult and If you only want to avoid passing some props through many levels, the component composition is often a simpler solution than context.

When to Use Context

Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language.

### Hooks and context example

After making an audit on how we communicate with our users, we landed with a simple system of three classes of communication, and snackbars fit perfectly on the ‘low priority’ end of that spectrum. They are small notifications that show up on the screen when a user performs an action. They are not intrusive at all and appear for just a brief moment.

This mean that we forget to render props and higher order components. We don’t want to deal with a messy React tree and wrappers. We don’t want action creators, reducers\*, or any of that stuff.

### When to Use Context

Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language.

Before You Use Context

Context is primarily used when some data needs to be accessible by many components at different nesting levels. Apply it sparingly because it makes component reuse more difficult.

Component composition is frequently a simpler option than context if you just want to avoid sending some props over multiple layers. What component type (class/function) should you use when you have numerous contexts, and why?
The distinction is unmistakable. Functional Components are functions while Class Components are ES6 classes. A functional component's only requirement is that it receive props as an argument and return acceptable JSX.
What is the best way to test context? Making our tests uninformed of Context's existence and avoiding mocks is the best approach to test it. We want to test our components in the same way that developers do (behavioral testing) and in the same way that they would operate in our environment.