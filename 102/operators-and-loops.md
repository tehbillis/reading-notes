# Operators And Loops

At a high level, and expression is a valid unit of code that resolves to a value. there are thow kinds of expressions:

1. Those that have side effets (Like assigning values).
2. Those that purely evaluate.

The precedence of operators determins the order they are applied when evaluating an expression.

JS Has both binary and urnary operators, as well as one special ternary operator, the conditional operator. A vinary operator requires two operands, one before and one after the operator. A urnary operator requires just one, it can be either before or after the operator.

## Assignment Operators

An assignment operator assign a value to its lefthand operand based on the value of its righthand operand. The simple assignment operator is =, but the full list can be seen below:

| Name                                 | Shorthand operator | Meaning                |
| ------------------------------------ | ------------------ | ---------------------- |
| Assignment                           | x = f()            | x = f()                |
| Addition assignment                  | x += f()           | x = x + f()            |
| Subtraction assignment               | x -= f()           | x = x - f()            |
| Multiplication assignment            | x *= f()           | x = x * f()            |
| Division assignment                  | x /= f()           | x = x / f()            |
| Remainder assignment                 | x %= f()           | x = x % f()            |
| Exponentiation assignment            | x **= f()          | x = x ** f()           |
| Left shift assignment                | x <<= f()          | x = x << f()           |
| Right shift assignment               | x >>= f()          | x = x >> f()           |
| Unsigned right shift assignment      | x >>>= f()         | x = x >>> f()          |
| Bitwise AND assignment               | x &= f()           | x = x & f()            |
| Bitwise XOR assignment               | x ^= f()           | x = x ^ f()            |
| Bitwise OR assignment                | x \|= f()          | x = x \| f()           |
| Logical AND assignment               | x &&= f()          | x && (x = f())         |
| Logical OR assignment                | x \|\|= f()        | x \|\| (x = f())       |
| Nullish coalescing assignment        | x ??= f()          | x ?? (x = f())         |

### Assigning to properties

If an expression evaluates to an object, then the lefthand side of an assignment expression may make assignments to properties of that expression. If an exdpression does not evaluate to an object, then assignments to properties of that expression don't assign.

### Destructuring

Syntax that makes it possible to extract data from arrays or objects using syntax that mirrors the construction of array and object literals.

Example without destructuring

```javascript
const foo = ["one", "two", "three"];

const one = foo[0];
const two = foo[1];
const three = foo[2];
```

Example with Destructuring

```javascript
const [one, two, three] = foo;
```

### Assignment chains

Are complicated and can result in surprising or unexpected behavior. They are typically avoided.

## Comparison Operators

A copmarison operator compares its operands and returns a logical value based on whether the comparison is true.

### List of Comparison Operators

| Operator                 | Description                                                    | Examples returning true |
| ------------------------ | -------------------------------------------------------------- | ----------------------- |
| Equal (==)               | Returns true if the operands are equal.                       | 3 == var1               |
|                          |                                                               | "3" == var1             |
|                          |                                                               | 3 == '3'                |
| Not equal (!=)           | Returns true if the operands are not equal.                   | var1 != 4               |
|                          |                                                               | var2 != "3"             |
| Strict equal (===)       | Returns true if the operands are equal and of the same type.  | 3 === var1              |
|                          | See also Object.is and sameness in JS.                        |                         |
| Strict not equal (!==)   | Returns true if the operands are of the same type but not equal, or are of different type. | var1 !== "3"            |
|                          |                                                               | 3 !== '3'               |
| Greater than (>)         | Returns true if the left operand is greater than the right operand. | var2 > var1             |
|                          |                                                               | "12" > 2                |
| Greater than or equal (>=)| Returns true if the left operand is greater than or equal to the right operand. | var2 >= var1           |
|                          |                                                               | var1 >= 3               |
| Less than (<)            | Returns true if the left operand is less than the right operand. | var1 < var2             |
|                          |                                                               | "2" < 12                |
| Less than or equal (<=)  | Returns true if the left operand is less than or equal to the right operand. | var1 <= var2           |
|                          |                                                               | var2 <= 5               |

## Loops

Loops offer a quick and easy way to do something repeatedly. There are many types of loops but they all do essentially the same thing, they repeat an action X number of times.

### For Loop

A `for` loop repeats until a specified condition evaluates to false. An example of a `for` loop that repeats 5 times would look like

```javascript
for(let i = 0; i < 5; i++) {
    //code
}
```

### While Loop

A `while` loop repeats as long as a specified condition remains true. An example of a `while` loop that repeats 3 times would look like

```javascript
let n = 0;
let x = 0;
while (n < 3) {
  n++;
  x += n;
}

```

## Answer

1. **What is an `expression` in JavaScript? -** A valid unit of code that resolves to a value.
2. **Why would we use a loop in our code? -** to repeat something multiple times.
3. **When does a `for` loop stop executing? -** when a specified conditions evalueates to false.
4. **How many times will a `while` loop execute? -** as long as the condition is true.
