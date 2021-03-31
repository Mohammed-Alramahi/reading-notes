# HTML Links, JS Functions, and Intro to CSS Layout

## HTML links

**We can make links using the anchor tag `<a href='path'>link text</a>` and it's pretty obvious how to make a link in HTML but what if we are linking an outside page or any different page inside our directories?**

|directory path      | Example                                             |
|--------------------|-----------------------------------------------------|
| Same folder        | `<a href='index.html'>Home page</a>`                |
| child folder       | `<a href='pages/about.html'>about page</a>`         |
| grandchild folder  | `<a href='public/pages/contact.html'>about page</a>`|
| parent folder      | `<a href='../index.html'>about page</a>`            |
| grandparent folder | `<a href='../../example.html'>about page</a>`       |


**When the specified link isn't correct it will give us an error of *404 page not found* .**

**What if we want to send an email through HTML? or we want the link to open in a new tab**

```html
   <!-- This is how to send an email -->
   <a href="mailto:someone@email.com">Contact someone</a>
   <!-- This is how to open link in new tab by giving a target attribute -->
   <a href="index.html" target="_blank">

```

**We can even put a link for the same page but on some location on the page by specifying the id of that element and this can come very handy when creating a user-friendly website:**

**Let's imagine that it's a long page with a lot of content inside of it we can for example make a link to navigate from top to bottom or the opposite.**

```html
   <div id="top-area"><a href="#bot-area">go down to bottom</a></div>
   <!--really long page with alot of content-->
   <div id="bot-area"><a href="#top-area">go back to top</a></div>
```

***

## CSS Layout

**building  blocks**
 - Inline elements: will flow inside the text like `<span>`.
 - Block-level elements: will cover a whole line of content and you can specify each space will the element cover like `<div>`
 - when there is a block-level element inside another block-level element it gonna treat the outside element as a parent element and you can change the space between them through *padding*.

 **For the positioning there are three types:**
 - Normal flow: each element will display after each other side by side or on top of each other.
 - Relative positioning: gonna shift the element top, bottom, left, and right depending on what you specified.
 - Absolute positioning: it gonna ignore any spaces between the elements and position them as you want.

 - `z-index` will make the element overlap other elements or sit behind them.
 - floating elements will make the element float on the page either right or left.
 ```css
 .card{
     position:relative;
     top: 50px;
     right: 30px;
     z-index: 1;
     float: left;
 }
 ```
***
## JS Functions

**Functions in javascript enable us to group a set of instructions so you can do something specific that is repetitive in your code without needing to write these instructions over and over so it's really helpful.**

```javascript 
  let number1=5;
  let number2=6;
  function summation()
  {
      let sum= number1+number2;
      return sum;
  }
  console.log(summation());
  //or you can make it as an anonymous function

  let sum= function(){
      return number1+number2;
  }
  console.log(sum);
```
