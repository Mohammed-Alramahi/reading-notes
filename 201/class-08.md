
### CSS Layout

**building blocks**

- Inline elements: will flow inside the text like `<span>`.
- Block-level elements: will cover a whole line of content and where you can give how much space will the element cover like `<div>`.
- when there are block-level elements inside each other,  it gonna treat the outside element as a parent element and you can specify the space between them through *padding*.

**the positioning has three types:**

- Normal flow: where each element will display after other elements side by side or on top of each other.

- Relative positioning: it will move the element top, bottom, left, and right depending on what you specified.

- Absolute positioning: it gonna ignore any spaces between the elements and you can position them the way you like.

- `z-index` will make the element sit behind other elements or overlap them.

- floating elements will make the element float on the page either right or left.

```css
.nav{
    position:absolute;
    top: 20px;
    right: 30px;
    z-index: 0;
    float: right;
}
```