# Interpreter made for Monkey Programming Language

[source](https://interpreterbook.com/)

## Some notes:
#### Chapter 2: Writing a parser**
- There are two types of parsers: top-down and bottom-up.
- The difference between top-down & bottom-up parsers is that the top-down parser starts with constructing the root node of the AST(Abstract Syntax Tree) and descends and the bottom-up does it the other way around.
- Recursive descent parsing, early parsing or predictive parsing are variations of top-down parsing.
- The parser that I wrote is a ***recursive descent parser***.
    - It is sometimes also called **Pratt parser**, 
    - It is "top-down operator precedence" 
- ***Note: Expressions produce values, statements don't***
    - `let x = 5;` doesn't produce a value but `5` produces a value 5
    - `return n;` is a statement it doesn't produces a value
    - `add(x,y)` is a function literal, it produces a value that it will return
    - It depends on the programming language and the choice its designers made, we are parsing for monkey programming language so fuction literals are expressions