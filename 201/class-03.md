# HTML Lists, CSS Boxes, JS Control Flow

## Lists:

**There are 3 types of lists in HTML that each one of them has it's own use but in overall they all work the same:**
 1. Ordered list: where every list item will be ordered numerically in default but it also can be alphabetically. And here is an example of how to make one:

  ```html
      <ol>
      <li>List item #1</li>
      <li>List item #2</li>
      <li>List item #3</li>
      </ol>
  ```

 2. Unordered list: where every list item may not be ordered and will be represented with bullet point.

  ```html
      <ul>
      <li>List item #1</li>
      <li>List item #2</li>
      <li>List item #3</li>
      </ul>
  ```

 3. Definition list: which will hold a series of definitions in a bit different way than OL and UL:

  ```html
        <!--Sources of terms below are all from google-->
        <dl>
        <dt>Html</dt>
        <dd>The HyperText Markup Language, or HTML is the standard markup language for documents designed to be displayed in a web browser.</dd>
        
        <dt>CSS</dt>
        <dd>Cascading Style Sheets is a style sheet language used for describing the presentation of a document written in a markup language such as HTML.</dd>

        <dt>Javascript</dt>
        <dd>JavaScript is high-level, often just-in-time compiled, and multi-paradigm.</dd>
        </dl>
  ```
**Note that lists also might be nested inside each other.**
***
## CSS boxes:

**Every element on any html page are considered as box where it has it's own properties like:**
 - width, max-width, min-width . where (max-width and min-width) will limit the box width.
 - height, max-height, min-height . as width (max-height and min-height) will limit the box height.
 - Overflow: make the browser have some overflow if the content was larger than the box then it will either hide the    extra content or add a scroll based on the giving value.
 - Every box has a border even if it wasn't visible to you it will have a default value of 0 but it's still there.
 - margin will be placed outside the border and it will set a gap between the boxes.
 - padding is like margin but it's gonna be inside the border and it will add space between it and the box itself.

  ```css
  header{
        width: 250px;  /*or min-width*/
        height: 400px; /*or max-height*/
        border: 2px solid #000000;
        padding: 10px;
        margin-left: 50px;
        overflow: hidden;
        text-align: center; 
    }
``` 
***

## Javascript switch:

**A `switch` works exactly like an `if` statement but it gonna do intructions if the variable that we are checking for has some value.**

 ```javascript
    let number=prompt('enter number between 1 and 3');
    switch(number)
    {
        case '1':
        document.write(1);
        break;
        case '2':
        document.write(2);
        break;
        case '3':
        document.write(2);
        break;
        default:
        alert('please enter number between 1 and 3 only');
    }
 ```
