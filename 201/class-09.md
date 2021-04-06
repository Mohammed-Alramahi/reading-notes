## HTML Forms

**Whenever we want to submit anything to server such as login information or search for something like in google all of these will depend on forms**

There are so many types of data that we can submit through forms like:
- a plain text like a facebook post or the one we use to search on google.
- a password we use in our credentials for signing up or in.
- a file like images or PDF files.
- making choices like gender when registering to a website.
- quizes on canvas are made up from forms.

And the list goes on.

**So how do we exactly make a form?**

```html
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
</head>

<body>
  <form method="POST" action="index.html">
    <input type="text" name="username">
    <input type="password" name="password">
    <input type="submit" name="submit">
  </form>
</body>

</html>
```
**What is method and action?**
- for the action it means what page are we submiting our data for.(this will propably be implemented with the backend)
- method is a way of specifying if that data is sensitive or not, for example if we are submiting a user credentials we don't want to use `method="GET"` because it will right any submitted data in the URL so we gonna use `method="POST"` because it will hide submitted information without showing it anywhere unless we tell it to.
***
## CSS Lists, Tables and Forms

**We can basically style our Lists, Tables and Forms as we want along with some other properties like:**
1. **for lists we can do**
 - `list-style:none;` which will remove any bulletpoints and this become handy when making a navbar for example
 - `list-style-image: url("img/listitem.png");` with this property we can add an image for our list item instead of having other pre defined styles like bullet points.
 - `line-height: 1.2em;` this will make some space between list items.
 - we can apply any text or color styles for the lists.

2. **for tables**
  -  `border-spacing: 0px;` we can change the whole box size of the table and this can be useful while using animations with the table.
  - `border-collapse: collapse;` we can set it to seperate as well but it's the default value for collapse and most of the time we want to use `border-collapse: collapse;` instead of `border-collapse: seperate;` because it have much more clear view of the cells in table.
  - we can apply any text or color styles for the tables as well.
3. **for forms**
  -we can do absolutely anything from our previous knowledge on CSS.

***
## Javascript Events

**Javascript events when used correctly can be overwhelmingly powerful because we can make the most of it when comes to dynamic design and interacting with user and there is no any successful website that doesn't utilize events.**

**So it will make any specific task upon a specific kind of interaction from users like clicking a button or moving the cursor at some position on screen and imagine going onto a website full of buttons that do nothing when clicking them will it make sense? of course no and after some event it will trigger a code that we specify also.**

**some examples of events:**
- load: when the page done loading process.
- unload: page unloading because other page is been requested (most of the time).
- click: when we mouse click on something.
- dblclick: when we make a double mouse click on something.
- scroll: while scrolling on the page.

 And the list goes on and on.

**steps for making an event up and running:**
1. specify an element.
2. specify the trigger. (maybe a mouse click)
3. run some code upon the trigger.

**This is an example of when user click button *x* then it will show him a message of "hello, there!"**
```javascript
let btn=document.getElementById('x').onclick= function(){
    alert('hello, there!');
}
```
**note:There are so many ways of making events but using the DOM is the best practice of all.**