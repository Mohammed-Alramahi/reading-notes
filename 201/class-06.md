 ## Why the Problem Domain Is The Hardest Part Of Programming
[link of the read](https://simpleprogrammer.com/understanding-the-problem-domain-is-the-hardest-part-of-programming)

**Why programming is so overwhelming? well, there are various answers to this question:**

- you will have to adopt new technologies.
- Naming stuff like variables and functions.
- Testing results of the code.
- Debugging (the process of finding bugs and fixing them).
- getting rid of bugs (if found).
- Making software scalable and maintainable.
- etc.

**To have the idea of how to solve a problem we should keep building the stuff over and over again and that's where we'll have familiarity with the problem domain.**

**What you can do to get rid of problem domain:**
- Make the problem domain simpler.
- Have a better understanding of the problem domain.
***
## Object literals

**Literal notation is the most common and considered the easiest way to create objects**

To get or set properties or methods of objects we gonna use dot `.` to implement that.

```javascript
 let todos={
     id:1,
     text:'study JS',
     isCompleted:false
 };
 console.log(todos.text,isCompleted);
```
**Conclusion: object literals are less complex, more efficient, and produce much cleaner code.**
***

## The document object model aka DOM

**DOM is a tree where every element, attribute, or text content is a *DOM node* .** 
**Accessing and modifying the DOM are done through two steps:**
- Locate the node that is specified as the element.
- Manipulate it as you want.

**Accessing the elements are achieved by:**

 1. Accessing a single node.
  - `getElementById()` given an id will return the element by it's ID.
  - `querySelector()` passing a CSS selector will return the element.
 2. Accessing multiple nodes.
  - `getElementsByClassName()` will give all elements holding that class attribute.
  - `getElementByTagName()` returns all elements with that tag like `<div>`
  - `querySelectorAll()` will return all possible elements that uses that CSS selector.
 3. Traversing between nodes.
  - `parentNode` selects the parent of the element.
  - `firstChild` select the first child of the current element.

 **Manipulating elements:**
 1. Access or update text.
 1. Manipulating HTML content.
 1. Updating attributes values.


 **Let's say I have this *'index.html'* file:**
 
 ```html
 <!DOCTYPE html>
<html>
<head>
    <title>index</title>
</head>
<body>
    <button id="add-text" type="button">add text</button>
    <p id="para1">
    
    </p>
    <script src="app.js"></script>
</body>
</html>
 ```
 **And I want to add some text to `para1` from my *'app.js'* file by clicking a button. It will go like this:**

 ```javascript
 document.getElementById('add').onClick=function(){
 document.getElementById('para1').innerHTML='Hello world!';
 };

 ```