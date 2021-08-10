# Component Lifecycle / useEffect() Hook

## Review, Research, and Discussion

### Why do we not need more .html pages in a multi-page React app?

In a multi-page react app, we don't need any additional html pages since we can use a browser router to render certain components on separate pathways using a browser router. This is due to the way React handles the DOM.

### If we wanted a component to show up on every page, where would we put it and why?

- **Inside the BrowserRouter , outside a Route**

### What does routing do with the components that were rendered when a new route is requested

  it goes to the new component and removes the old component from the DOM.

### What does props.children contain?

  props.children is a children that were passed to the component.

### How do useState() and this.setState() differ?

  setState is merging the previous state with the new one, it means that you dont have to pass the full state object every time you want to change some part of the state. React will update given properties and won’t touch the rest. The useState’s updater rewrites a previous state with a new one and it does not perform any merging. Its just replacement instead of merging.

## Document the following Vocabulary Terms

- **State Hook** is a Hook that allows you to have state variables in functional components , it takes the initial state as an argument and returns an array of two entries.

- **Mounting and Un-Mounting** The main job of React is to figure out how to modify the DOM to match what the components want to be rendered on the screen. React does so by mounting (adding nodes to the DOM), unmounting (removing them from the DOM), and updating (making changes to nodes already in the DOM).

## Preparation Materials

### Using the Effect Hook

  **What does useEffect do?** By using this Hook, you tell React that your component needs to do something after render. React will remember the function you passed (we’ll refer to it as our “effect”), and call it later after performing the DOM updates. In this effect, we set the document title, but we could also perform data fetching or call some other imperative API.

  **Why is useEffect called inside a component?** Placing useEffect inside the component lets us access the count state variable (or any props) right from the effect. We don’t need a special API to read it — it’s already in the function scope. Hooks embrace JavaScript closures and avoid introducing React-specific APIs where JavaScript already provides a solution.

  **Does useEffect run after every render?** Yes! By default, it runs both after the first render and after every update. (We will later talk about how to customize this.) Instead of thinking in terms of “mounting” and “updating”, you might find it easier to think that effects happen “after render”. React guarantees the DOM has been updated by the time it runs the effects.