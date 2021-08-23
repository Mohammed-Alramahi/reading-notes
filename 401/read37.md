# Redux - Combined Reducers

## Review, Research, and Discussion


* **Why choose Redux instead of the Context API for global state?**

Redux is the industry standard for managing state of large applications, so it is important to know well. It is more optimized for larger projects, because the context API re-renders more often.

* **What is the purpose of a reducer?**

We need reducers to tell the application how to change state in response to an action. The action does not do anything except describe what happened and it is up to the reducer to respond to this.

* **What does an action contain?**

An action contains a type and whatever payload you want it to have. There is flexibility in what there is besides the type.

* **Why do we need to copy the state in a reducer?**

The reducer needs to be a pure function without any side-effects. It should only take in an action and return the new state, but it should not mutate the state, so we need to copy it to update it.

## Document the following Vocabulary Terms

* **immutable state:** This allows the state to only change when absolutely necessary to make React apps perform as well as possible.

* **time travel in redux:** This is a feature of redux dev tools that allows you to see every state that a page has been in.

* **action creator:**	Actions send data from your application to your store, and are the only source of information for the store. An action creator is a function that creates an action.

* **reducer:** Reducers tell the application how to change state in response to an action.
* **dispatch:** This is the name of the function you use to send actions to the store.

## Preparation Materials

### *Using combineReducers*

* **Core Concepts:**
A simple Javascript object containing "slices" of domain-specific data at each top-level key is the most typical state form for a Redux app. Similarly, the most popular method to building reducer logic for that state shape is to use "slice reducer" functions, each with the same (state, action) signature and each in charge of managing all modifications to that slice of state. Multiple slice reducers can respond to the same action, updating their own slice as appropriate, and then combining the changed slices into the new state object.

Because this pattern is so common, Redux provides the combineReducers utility to implement that behavior. It is an example of a higher-order reducer, which takes an object full of slice reducer functions, and returns a new reducer function.


* **Defining State Shape**

The initial shape and contents of your store's state may be defined in two ways. First, preloadedState can be sent as the second parameter to the createStore method. This is mostly used to populate the store with data that was previously saved somewhere else, such the browser's localStorage. When the state parameter is undefined, the root reducer might also return the original state value. These two techniques are discussed in further depth in Initializing State, however when utilizing combineReducers, there are some extra considerations to keep in mind.
combineReducers generates a function that outputs a similar state object with the same keys from an object containing slice reducer functions. If createStore is not given a preloaded state, the naming of the keys in the input slice reducer object will be used to name the keys in the output state object. When utilizing ES6 features like default module exports and object literal shorthands, the relationship between these names isn't always obvious.