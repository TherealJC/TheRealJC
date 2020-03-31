# Code Camp JS

 In computer science, data is anything that is meaningful to the computer. JavaScript provides seven different data types which are `undefined`, `null`, `boolean`, `string`, `symbol`, `number`, and `object`.

Assignment always goes from right to left. Everything to the right of the `=` operator is resolved before the value is assigned to the variable to the left of the operator.

`i++;`is the equivalent of`i = i + 1;`   The entire line becomes `i++;`eliminating the need for the equal sign.  The remainder operator `%` gives the remainder of the division of two numbers.

 Like the `+=` operator, `-=` subtracts a number from a variable. myVar = myVar - 5; will subtract `5` from `myVar`. This can be rewritten as: `myVar -= 5;`

 `"your name"` is called a string literal. It is a string because it is a series of zero or more characters enclosed in single or double quotes.

When you are defining a string you must start and end with a single or double quote. What happens when you need a literal quote: `"` or `'` inside of your string? ``In JavaScript, you can escape a quote from considering it as an end of string quote by placing a backslash \(`\`\) in front of the quote.`var sampleStr = "Alan said, \"Peter is learning JavaScript\".";`

```text
var myStr = "I am a \"double quoted\" string inside \"double quotes\".";
Pay attention to how it ends with the last " outside the \ (\"----\") and the 
position of the .
```

 In JavaScript, when the `+` operator is used with a `String` value, it is called the concatenation operator. You can build a new string out of other strings by concatenating them together.

 You can find the length of a `String` value by writing `.length` after the string variable or string literal.

With JavaScript `array` variables, we can store several pieces of data in one place. You start an array declaration with an opening square bracket, end it with a closing square bracket, and put a comma between each entry, like this: `var sandwich = ["peanut butter", "jelly", "bread"]`.

 You can also nest arrays within other arrays, like this: `[["Bulls", 23], ["White Sox", 45]]`. This is also called a multi-dimensional array. Unlike strings, the entries of arrays are mutable and can be changed freely.                                               var ourArray = \[50,40,30\];           ourArray\[0\] = 15;           // equals \[15,40,30\]

An easy way to append data to the end of an array is via the `push()` function. `.push()` takes one or more parameters and "pushes" them onto the end of the array.

```text
var arr = [1,2,3];
arr.push(4);
// arr is now [1,2,3,4]
```

 That's where `.shift()` comes in. It works just like `.pop()`, except it removes the first element instead of the last.  `.unshift()` works exactly like `.push()`, but instead of adding the element at the end of the array, `unshift()` adds the element at the beginning of the array.

**Parameters** are variables that act as placeholders for the values that are to be input to a function when it is called. When a function is defined, it is typically defined along with one or more parameters. The actual values that are input \(or "passed"\) into a function when it is called are known as arguments.

Here is a function with two parameters, `param1` and `param2`:

```text
function testFun(param1, param2) {
  console.log(param1, param2);
}
```

Then we can call `testFun`: `testFun("Hello", "World");` We have passed two arguments, `"Hello"` and `"World"`. Inside the function, `param1` will equal "Hello" and `param2` will equal "World". Note that you could call `testFun` again with different arguments and the parameters would take on the value of the new arguments.

 `If` statements are used to make decisions in code. The keyword `if` tells JavaScript to execute the code in the curly braces under certain conditions, defined in the parentheses. These conditions are known as `Boolean` conditions and they may only be `true` or `false`.

