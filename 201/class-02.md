# Basics of HTML, CSS & JS

### HTML tags

**HTML tags come as two types *the structural markup* and *the semantic markup* where semantic tags were present in HTML5**

HTML headings go all the way from `<h1>` to `h6` where the most priority is for `<h1>` and the text goes smaller as we go towards `<h6>`.

To write a paragraph use the `<p>` tag. You can also customize some of the text attributes like `<b>` tag will make your text bolder and `<i>` will make it italic and this will go through HTML only without using CSS.

Browsers will ignore your new lines in HTML and consider it as a single white space, but you can use `<br>` or `<hr>` to whitespace by one line.

All of the tags present above are considered as *Structural markup* tags. For *Semantic markup* tags there is a bunch of tags that we can use to style our text like `<strong>` which will do the same as `<b>` but it's written semantically to illustrate more about the content. There are also tags like `<abbr>` which we will use to demonstrate an abbreviation, `<address>` tag will contain some contact information about the author.
***
### CSS intro
CSS enables you to make rules that control the way that every individual box is presented and the look of it.
**Every CSS rule has consist of two parts the selector and the declaration here is an example:**

```css
 p{
     color:red;
 }
```
where `p` is the selector and `color:red` is the declaration.

**There are 3 ways of writing CSS:**
 - Inline. (not recommended)
 - Internal. (not recommended)
 - External. (the most practical way) by linking the source to the CSS file 
  ```html
   <head>
   <link rel="stylesheet" href="style.css">
   </head>
  ```
**CSS selectors:**
 | Selector   | Example  |     Funcion                                                                 | 
 | -----------| ---------|-----------------------------------------------------------------------------| 
 | Universal  |  `*{}`   | Will apply the style for every element in the page                          |
 | Type       |   `p`    | Will apply the style for every `p` tag in the page                          |
 | Class      |  `.card` | Will apply the style for every element that hold `card` class in the page   |
 | ID         |  `#main` | Will apply the style only for the element that hold `main` id in the page   |
***
### So how do we write JS code?

**Some of the JS datatypes:**
 - Strings.
 - Numbers. (integers and floating-point numbers)
 - Booleans.

 **JS variable naming rules:**
 - The first character of the variable name should be a letter or an underscore (_) only.
 - Mustn't start with a number.
 - Should notice that JS is a case-sensitive language.
 - Utilize *Camel case* technique. by writing all lowercase except for the first character of the second word in the variable if presented like `var pageUrl;`
 - Don't use keywords in names solely. for instance `var let=5;`.
 - No whitespaces. (Use dash - instead)


**This is an example of very basic JS code which will either add or subtract two numbers and print them onto page based on the met condition using `if`:**

```javascript
  //Simple calculator
  let number1 = 5;
  let number2 = 10;
  if(number1 >= number2)
  {
     document.write(number1+number2); 
  }
  else{
      document.write(number2-number1); 
  }

```