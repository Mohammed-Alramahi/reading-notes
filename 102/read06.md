## Introducing CSS

 *CSS rules:* Any CSS rule will be a combination of both selector and a declaration where selector will identify  which element are we styling and declaration will have 2 parts (property & value) where property what the style that we want to change color for specific element and the value will be red for instance:
 `p{`
 `color:red;`
 `}`
- The selector could be either class, id, or the element name itself ex:`h1`.
- While you can write CSS code inside HTML document it's always preferred to separate it in a split file.(*best practices*)
***
# Colors in CSS
>Colors in computers generally work on a system called RGB by mixing up Red, Green and Blue colors which make up about 16.7 million possible RGB color combinations. -source: (Google)
***
*Ways of representing colors in CSS:*

*Foreground colors*
- By writing the color name.
`h1{`
 `color: white;`
`}`
- By writing the hexadecimal value of the color.
`h1{`
 `color:#ffffff;` (white color in hex value)
`}`
- By writing the RGB values (Red Green Blue).
`h1{`
 `color:RGB(255,255,255)` (white color in RGB values)
`}`
***
*Background colors*
- *Same goes as above, but we change `color` into `background-color` and that's pretty much it.*
***
*The Most important thing while playing around with colors is the contrast because when you have let's say yellow background and pink foreground color you will immediately notice how it's ugly and unreadable at the same time so keep that in mind.*
***
*CSS has added extra value for RGB system that specifies opacity. Which is known as RGBA where a stands for alpha*
