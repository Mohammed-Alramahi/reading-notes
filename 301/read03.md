 # Passing Functions as Props

 **What does map return?**
 
  It return a new array from an existing array based on some rules. 
  
  ```javascript
    let names=['ali','rana','mohammad'];
    let newNames=names.map(name=>{
        return 'hello '+name;
    });
    //the code above will take every element inside names array and 'hello' before it and make new array based on it.
  ```

 **If I want to loop through an array and display each value in JSX, how do I do that in React?**

 This is an example of how to use map in React. 

```jsx
  let names=['ali','rana','mohammad'];
  const namesList = names.map((name) =>{
    <li key={name.toString()}></li>
    {name}
  });
```

 **Each list item needs a unique _**

 It will need a unique key among other siblings.

 **What is the purpose of a key?**

 We use keys to make hints to React.

***

 **What is the spread operator?**

 It's `...` that is used to expand an iterable object to a list of arguments.

 **What spread operator can do?**

 - Copy an array.
 - Concatenate arrays or combine them.
 - Using math functions.
 - Adding a state in React.

 **Give an example of using the spread operator to combine two arrays.**

  ```javascript
  const firstArray = [`1`,`2`,`3`]
  const  secondArray= [`4`,`5`,`6`]
  const resultArray = [...firstArray,...secondArray];
  console.log(...resultArray) //1 2 3 4 5 6
  ```

  **Give an example of using the spread operator to add a new item to an array.**

  ```javascript
  const names=['mohammed','ali','rana'];
  const newNames=['khalid','samer',...names]
  console.log(newNames);
  ```

  **Give an example of using the spread operator to combine two objects into one.**

  ```javascript
  const firstObject={name:"mohammed",age:23};
  const secondObject={major:"CS",isCool:true};
  const resultObject={...firstObject,...secondObject};
  console.log(newNames);
  ```
  
***

  ## Things I want to know more about

  - Spread operator.
  - Props and states.
  - React Bootstrap.
