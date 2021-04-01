# HTML Images; CSS Color & Text

### Images 

**While choosing the Images for your website:**
- Try to be relevant while choosing images.
- Make it benificial or meaningful.
- Let it be convenient for you website.
- Fit the colors template in your website.

**How to add Images in HTML**

```html
 <p>Some text............</p>
 <img src="img1.png" alt="alternative" width="500px" height="500px"/>
```
**note that it's a self closing tag which means it doesn't require an closing tag.**

**There are alot of image formats but the most important or more common formats in web are:**
- JPEG.
- PNG.
- GIF.


**It's more suitable to save your photos as JPEG and you logos or illustrations as a GIF.**

***
### CSS Colors

**We can specify colors in various ways in CSS:**
- RGBA value:`color:rgba(255,255,255,1)` where A is alpha which is opacity.
- Hex value: `color:#ffffff` which represent white color in hexadecimal value.
- Color name:`color:red` this one is pretty obvious.
- HSL value:`hsl(0, 80%, 60%)`. Hue, Saturatino and Lighting.
 
**The most important thing when choosing a color is considering other elements colors you need to make them all work smooth together and don't make silly mixes.**

**Background and Foreground colors:**

```css
 p{
     background-color:#ffffff;
     color:#000000; /*This one is for foreground and the one on top are background*/
 }
```
**We can always consider using color pickers software which is widely common online, personally i prefer using the VS Code color picker.**

***
### CSS Text

**There are many ways to use fonts you can either choose from the local one or online font but bare in mind that if you want to use an online font you can't actually use it before importing it just like a normal CSS file**

**Font family:it enables you to choose the typeface that should be applied for any text inside the elements.**

**You can specify `font-size` by pixels or percentages (responsive design) and you can apply it as above.**

**Font weight: like normal as default or bold which will make it bigger and kinda darker.**

**Font style: like normal,italic and oblique which will make different variations of the style.**

**`text-transform` with this property you can either make your text all uppercase or all lowercase or finally capitalize the first letter in each word.**

**`text-decoration` property has values of underline,overline, line through and none. which is all obvious and self-explained**

**`text-align` which has four possible values: left, justify, center and right . And with justify this would be an indication of that every line in a paragraph should take the whole width except for the last line.**

```css
 body{
     font-family: Arial, Helvetica, sans-serif;
     font-size: 36px;
     weight:bold;
     font-style:italic;
     text-transform:capitalize;
     text-decoration:none;
     text-align:center;
```
