# Operators and Loops in JS

*Types of operators that evaluate conditions:(All of them return true values)*
- "Equal" to `==` will just compare values without comparing the data type. `'Welcome'=='Welcome'`
- "Not equal to" `!=` will just compare values without comparing the data type. `'Welcome'=='Hello'`
- "Strictly equal to" `===` will compare values and the data type. `9 === 9`
- "Strictly not equal to" `!==` will compare values and the data type. `'77' !== 77`
***
*There are also some other types of comparison like:(All of them return true values)*
- "Greater than" `>` . ex. `5>4`
- "Less than" `<` . ex. `4<5`
- "Greater than or equal to" `>=` . ex. `45>=43`
- "Less than or equal to" `<=` . ex. `50<=50`
***
*We can also compare between two expressions using Logical operators and here some examples:*
- This one will return *true* only if both expressions are *true* `((77<88) && (55==55))`
- This one will return *true* if one of the expressions are *true* `(('Khalid'=='Khaled')) || ('Ali'=='Ali'))`
While the first expression is *false* the second one is *true* Which will return *true* from both expressions.
- This statement will work in opposite manner `!` which will return *true* when the result is true and return *false* when the result is *true*.
## This table will explain more about the earlier section:

 | operator   |   expression #1    |   expression #2    |  result    |
 | -----------| -------------------|--------------------|------------| 
 |  `&&`      |      `true`        |     `true`         |  `true`    |
 |  `&&`      |      `false`       |     `true`         |  `false`   |
 |  `&&`      |      `true`        |     `false`        |  `false`   |  
 |  `&&`      |      `false`       |     `false`        |  `false`   |
 |  `\|\|`    |      `true`        |     `true`         |  `true`    |
 |  `\|\|`    |      `false`       |     `true`         |  `true`    |
 |  `\|\|`    |      `true`        |     `false`        |  `true`    |  
 |  `\|\|`    |      `false`       |     `false`        |  `false`   |
 |  `!`       |      `true`        |         -          |  `false`   |
 |  `!`       |      `false`       |         -          |  `true`    |

***
*what is a loop?*
 It's a set of instructions that will run repeatedely until a specific condition becoming no longer true.
 *Types of loops in JS:*
 - `for`
 - `while`
 - `do while`
***
*How to write for loop?*
 
  `var number=0;`
  `for (var counter=0;counter<5;counter++)`
  `{`
      `number++;`
  `}`
***
 *How to write while loop?*

  `while (number<10)`
  `{`
      `document.write(number)+<br>;`
      `number++;`
  `}`
  