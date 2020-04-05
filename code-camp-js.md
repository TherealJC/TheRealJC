---
description: Helpful Tips from Basic Javascript on FreeCodeCamp
---

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

Strict equality \(`===`\) is the counterpart to the equality operator \(`==`\). However, unlike the equality operator, which attempts to convert both values being compared to a common type, the strict equality operator does not perform a type conversion.

If the values being compared have different types, they are considered unequal, and the strict equality operator will return false.

 The inequality operator \(`!=`\) is the opposite of the equality operator. It means "Not Equal" and returns `false` where equality would return `true` and _vice versa_. Like the equality operator, the inequality operator will convert data types of values while comparing.

 The strict inequality operator \(`!==`\) is the logical opposite of the strict equality operator. It means "Strictly Not Equal" and returns `false` where strict equality would return `true` and _vice versa_. Strict inequality will not convert data types.

 The greater than operator \(`>`\) compares the values of two numbers. If the number to the left is greater than the number to the right, it returns `true`. Otherwise, it returns `false`.

 The greater than or equal to operator \(`>=`\) compares the values of two numbers. If the number to the left is greater than or equal to the number to the right, it returns `true`. Otherwise, it returns `false`.

 Sometimes you will need to test more than one thing at a time. The logical and operator \(`&&`\) returns `true` if and only if the operands to the left and right of it are true.  
The same effect could be achieved by nesting an if statement inside another if:

```text
if (num > 5) {
  if (num < 10) {
    return "Yes";
  }
}
return "No";
```

will only return "Yes" if `num` is greater than `5` and less than `10`. The same logic can be written as:

```text
if (num > 5 && num < 10) {
  return "Yes";
}
return "No";
```

 The logical or operator \(`||`\) returns `true` if either of the operands is `true`. Otherwise, it returns `false`.

When a condition for an `if` statement is true, the block of code following it is executed. What about when that condition is false? Normally nothing would happen. With an `else` statement, an alternate block of code can be executed.

```text
if (num > 10) {
  return "Bigger than 10";
} else {
  return "10 or Less";
}
```

If you have multiple conditions that need to be addressed, you can chain `if` statements together with `else if` statements.

```text
if (num > 15) {
  return "Bigger than 15";
} else if (num < 5) {
  return "Smaller than 5";
} else {
  return "Between 5 and 15";
}
```

If you have many options to choose from, use a switch statement. A `switch` statement tests a value and can have many case statements which define various possible values. Statements are executed from the first matched `case` value until a `break` is encountered.

Here is an example of a `switch` statement:

```text
switch(lowercaseLetter) {
  case "a":
    console.log("A");
    break;
  case "b":
    console.log("B");
    break;
}
```

`case` values are tested with strict equality \(`===`\). The `break` tells JavaScript to stop executing statements. If the `break` is omitted, the next statement will be executed.

If the `break` statement is omitted from a `switch` statement's `case`, the following `case` statement\(s\) are executed until a `break` is encountered. If you have multiple inputs with the same output, you can represent them in a `switch` statement like this:

```text
switch(val) {
  case 1:
  case 2:
  case 3:
    result = "1, 2, or 3";
    break;
  case 4:
    result = "4 alone";
}

Cases for 1, 2, and 3 will all produce the same result.
```



If you have many options to choose from, a `switch` statement can be easier to write than many chained `if`/`else if` statements. The following:

```text
if (val === 1) {
  answer = "a";
} else if (val === 2) {
  answer = "b";
} else {
  answer = "c";
}
```

can be replaced with:

```text
switch(val) {
  case 1:
    answer = "a";
    break;
  case 2:
    answer = "b";
    break;
  default:
    answer = "c";
}
```

Sometimes people use an if/else statement to do a comparison, like this:

```text
function isEqual(a,b) {
  if (a === b) {
    return true;
  } else {
    return false;
  }
}
```

But there's a better way to do this. Since `===` returns `true` or `false`, we can return the result of the comparison:

```text
function isEqual(a,b) {
  return a === b;
}
```

You may have heard the term `object` before.

Objects are similar to `arrays`, except that instead of using indexes to access and modify their data, you access the data in objects through what are called `properties`.

Objects are useful for storing data in a structured way, and can represent real world objects, like a cat.

Here's a sample cat object:

```text
var cat = {
  "name": "Whiskers",
  "legs": 4,
  "tails": 1,
  "enemies": ["Water", "Dogs"]
};
```

In this example, all the properties are stored as strings, such as - `"name"`, `"legs"`, and `"tails"`. However, you can also use numbers as properties. You can even omit the quotes for single-word string properties, as follows:

```text
var anotherObject = {
  make: "Ford",
  5: "five",
  "model": "focus"
};
```

However, if your object has any non-string properties, JavaScript will automatically typecast them as strings.  


You can add new properties to existing JavaScript objects the same way you would modify them.

Here's how we would add a `"bark"` property to `ourDog`:

`ourDog.bark = "bow-wow";`   or

`ourDog["bark"] = "bow-wow";`

Now when we evaluate `ourDog.bark`, we'll get his bark, "bow-wow".

Example:

```text
var ourDog = {
  "name": "Camper",
  "legs": 4,
  "tails": 1,
  "friends": ["everything!"]
};

ourDog.bark = "bow-wow";
```



Objects can be thought of as a key/value storage, like a dictionary. If you have tabular data, you can use an object to "lookup" values rather than a `switch` statement or an `if/else` chain. This is most useful when you know that your input data is limited to a certain range.

Here is an example of a simple reverse alphabet lookup:

```text
var alpha = {
  1:"Z",
  2:"Y",
  3:"X",
  4:"W",
  ...
  24:"C",
  25:"B",
  26:"A"
};
alpha[2]; // "Y"
alpha[24]; // "C"

var value = 2;
alpha[value]; // "Y"
```

