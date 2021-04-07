## Javascript Debugging

**The word debugging means find and fix errors and this apply to almost every programming language in the entire world and not only in javascript**


**Execution context consists of:**
- Global context where it's not sitting in any function or a specific block it's just there on js file.

- Function context will apply to what inside a function.

- Global Scope: If a variable is sitting outside a function, then it can be manipulated Globally because it's not in a specific scope.

- Function level scope what is inside a function can only be used inside a function and that applies in other programming languages too.

**The error consists of:**
- Name.
- Message.
- File number.
- Line number.


**Error objects and types:**
- Error as a general error where other errors depend on this object.
- Syntax Error when there is a missing curly brace for instance.
- Reference Error can be found when trying to use an un-existed variable.
- TypeError trying to use an inconvenient variable type.
- Range Error out of numbers ranges for example.


**we can use Devtools that is inside most modern websites by logging different types of messages for testing various results or logging errors.**

**we use `try catch` in to through exceptions when an error happens and that is called exception handling.**