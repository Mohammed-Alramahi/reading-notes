# Putting it all together

 **How would you break a mock into a component heirarchy?**
  
  drawing boxes around components in the mock and give them names.


 **What is the single responsibility principle and how does it apply to components?**
  
  Meaning a component should ideally only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents.


 **What does it mean to build a ‘static’ version of your application?**

  By using props only and not using states at all. States will be reserved only for interacting with users.


 **Once you have a static application, what do you need to add?**

 Adding states to make the UI interactive again.


 **What are the three questions you can ask to determine if something is state?**

 1. Is it passed in from a parent via props?
 2. Does it remain unchanged over time?
 3. Can you compute it based on any other state or props in your component?


 **How can you identify where state needs to live?**

 - Identify every component that renders something based on that state.
 - Find a common owner component (as a parent component)
 - Either the common owner or another component higher up in the hierarchy should own the    state.
- If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state.

## Things I want to know more about
 - States
 - Props
 - Components