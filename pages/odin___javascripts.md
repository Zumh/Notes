- ## Fundamental-1
  collapsed:: true
	- [Name the three ways to declare a variable](https://www.theodinproject.com/lessons/foundations-fundamentals-part-1#variable-declaration)
		- three variable that use in js
		  * var
		  * let
		  * const
	- [Which of the three variable declarations should you avoid and why?](https://www.theodinproject.com/lessons/foundations-fundamentals-part-1#avoid-var)
		- we should avoid var because var behavior can be confusing and unstable.
	- [What rules should you follow when naming variables?](https://javascript.info/variables#variable-naming)
		- Two rules to follow when naming variables
		  * The name must contain only letters, digits, or the symbols `$` and `_`.
		  * The first character must not be a digit.
	- [What happens when you add numbers and strings together?](https://javascript.info/operators#string-concatenation-with-binary)
		- one of operand is string then it concatenate and transform as string
	- [How does the Modulo (%), or Remainder, operator work?](https://javascript.info/operators#remainder)
		- The result of `a % b` is the remainder of the integer division of `a` by `b`.
	- [Explain the difference between `==` and `===`.](https://www.w3schools.com/js/js_numbers.asp)
		- difference in == and ===
		  * == attempt to convert and compare operands that are different 
		  * === strictly compare values and types of variables
	- [When would you receive a `NaN` result?](https://www.w3schools.com/js/js_numbers.asp)
		- `NaN` is a JavaScript reserved word indicating that a number is not a legal number.
	- [How do you increment and decrement a number?](https://javascript.info/operators#increment-decrement)
		- increment and decrement
		  number++ or number += 1
		  number-- or number -= 1
	- [Explain the difference between prefixing and postfixing increment/decrement operators.](https://javascript.info/operators#increment-decrement)
		- prefixing and postfixing
		  * prefix increment ++number or post fix increment number++
		  * prefix decrement --number or post fix increment number--
	- [What is operator precedence and how is it handled in JS?](https://javascript.info/operators#operator-precedence)
		- operator precedence is priority order of operators
	- [How do you access developer tools and the console?](https://www.theodinproject.com/lessons/foundations-fundamentals-part-1#access-devTools-console)
		- Access developer tools
		  * right click on web page and go to inspect or inspect Element.
		  * in the Developer Tools pane select Console tab.
	- [How do you log information to the console?](https://www.theodinproject.com/lessons/foundations-fundamentals-part-1#console-log)
		- console.log() is use for log info in the console.
	- [What does unary plus operator do to string representations of integers? eg. +”10”](https://javascript.info/operators#numeric-conversion-unary)
		- unary plus operator convert the string to integer
- ## Fundamental-2
  collapsed:: true
	- [What are the eight data types in JavaScript?](https://javascript.info/types#summary)
		- Eight data types
		  * number - integer $\frac{+}{-}(2^{53}-1)$ , float or any kind of numbers
		  * bigint - integer numbers of arbitrary length.
		  * string - for strings
		  * boolean - true or false
		  * null - for unknown values
		  * undefined - for unassigned values
		  * symbol for unique identifiers
		  * object for data structure
	- [Which data type is NOT primitive?](https://javascript.info/types#objects-and-symbols)
		- object is non-primitive data types
	- [What is the relationship between null and undefined?](https://javascript.info/types#the-null-value)
		- null vs undefined
		  * undefined - variable is declared but not assigned
		  * null - it just is own types that represent empty or nothing
	- [What is the difference between single, double, and backtick quotes for strings?](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/Strings#single_quotes_vs._double_quotes)
		- quotes
		  * single and double doesn't have big difference but must be consistence for readability
		  * backtick quote allow us to include variable inside the quote
	- [What is the term for embedding variables/expressions in a string?](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/Strings#concatenating_strings)
		- template literal is the term for use for joining variables.
	- [Which type of quote lets you embed variables/expressions in a string?](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/Strings#concatenating_strings)
		- In this case we use backtick quote allow us to embed variables/expressions.
	- [How do you embed variables/expressions in a string?](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/Strings#concatenating_strings)
		- ```js
		  const one = "Hello, ";
		  const two = "how are you?";
		  const joined = `${one}${two}`;
		  console.log(joined); // "Hello, how are you?"
		  
		  ```
	- [How do you escape characters in a string?](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/Strings#escaping_characters_in_a_string)
		- ```js
		  const bigmouth = 'I\'ve got no right to take my place…';
		  console.log(bigmouth);
		  ```
	- [What is the difference between the slice/substring/substr string methods?](https://www.w3schools.com/js/js_string_methods.asp)
		- Difference in slice, substring, substr
		  * slice - extracts a part of a string and returns the extracted part in a new string.
		  ```js
		  let text = "Apple, Banana, Kiwi";
		  let part = text.slice(7,13);
		  Banana
		  ```
		  * substring - start and end values less than 0 are treated as 0
		  * substr -  the second parameter specifies the **length** of the extracted part.
	- [What are the three logical operators and what do they stand for?](http://javascript.info/logical-operators)
		- Three logical operators
		  * && - AND
		  * || - OR
		  * ! - NOT
	- [What are the comparison operators?](https://javascript.info/comparison)
		- Comparison Operators
		  * > < - greater or less
		  * >= - greater or less than or equals 
		  * == - equal
		  * != - not equal
	- [What are truthy and falsy values?](https://javascript.info/ifelse#boolean-conversion)
		- truthy and falsy values are type conversions comparison in if statement.
	- [What are the falsy values in JavaScript?](https://javascript.info/ifelse#boolean-conversion)
		- falsy vs truthy
		  * falsy - 0, "", null, undefined, NaN, false
		  * truthy - other values
	- [What are conditionals?](https://www.w3schools.com/js/js_if_else.asp)
		- perform different actions for different decisions
	- [What is the syntax for an if/else conditional?](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/conditionals#basic_if...else_syntax)
		- ```js
		  if (condition){
		  } else if (condition) {
		  } else {
		  }
		  ```
	- [What is the syntax for a switch statement?](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/conditionals#switch_statements)
		- ```js
		  switch (expression) {
		    case choice1:
		      break;
		    default:
		  }
		  ```
	- [What is the syntax for a ternary operator?](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/conditionals#ternary_operator)
		- ```
		  condition ? run this code : run this code instead
		  
		  // toggle color black vs white
		  select.addEventListener('change', () => select.value === 'black'
		    ? update('black', 'white')
		    : update('white', 'black')
		  );
		  ```
	- [What is nesting?](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/conditionals#nesting_if...else)
		- Nesting
		  * Nesting code statement repeat itself more than one
		  * we can have if statement within another if statement
		  * for loop within another for loop etc...
- ## JavaScript Developer Tools
  collapsed:: true
	- [How do you open developer tools?](https://www.theodinproject.com/lessons/foundations-javascript-developer-tools#opening-dev-tools)
		- Open Js Dev Tools
		  * From the `Chrome Menu` > `More Tools` > `Developer Tools`
		  * Right-click anywhere on a webpage and select `Inspect`
	- [How do you change screen size of a website using developer tools?](https://developer.chrome.com/docs/devtools/device-mode/)
		- Drag the handles to resize the viewport to whatever dimensions you need. Or, enter specific values in the width and height boxes.
	- [What is a breakpoint?](https://developer.chrome.com/docs/devtools/javascript/breakpoints/)
		- break point is when the javascript pause while the code is running.
		- | Breakpoint Type | Use This When You Want To Pause... |
		  | [Line-of-code](https://developer.chrome.com/docs/devtools/javascript/breakpoints/#loc) | On an exact region of code. |
		  | [Conditional line-of-code](https://developer.chrome.com/docs/devtools/javascript/breakpoints/#conditional-loc) | On an exact region of code, but only when some other condition is true. |
		  | [DOM](https://developer.chrome.com/docs/devtools/javascript/breakpoints/#dom) | On the code that changes or removes a specific DOM node, or its children. |
		  | [XHR](https://developer.chrome.com/docs/devtools/javascript/breakpoints/#xhr) | When an XHR URL contains a string pattern. |
		  | [Event listener](https://developer.chrome.com/docs/devtools/javascript/breakpoints/#event-listeners) | On the code that runs after an event, such as `click`, is fired. |
		  | [Exception](https://developer.chrome.com/docs/devtools/javascript/breakpoints/#exceptions) | On the line of code that is throwing a caught or uncaught exception. |
		  | [Function](https://developer.chrome.com/docs/devtools/javascript/breakpoints/#function) | Whenever a specific function is called. |
	- [How do you set a breakpoint?](https://developer.chrome.com/docs/devtools/javascript/breakpoints/#loc)
		- Break points
		  * Sources > Open file > goto line of code > click on line number and blue icon appear
		  * Sourecs > Open file > goto line of code > right click > select Add condiitonal break points