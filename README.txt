1. Give three examples of Python programs that use binary operators and/or builtins from this PA, but have different behavior than your compiler. For each, write:
    a sentence about why that is
    a sentence about what you might do to extend the compiler to support it
    Ans:
    1) max(print(4),2)
       Python will have a compile error on this code but our compiler will return 4.
       To support it, we should check the input source of builtin2 and return ERROR if it is nested with "print".
    2) 2**4
       Python will compute the power and return 16, but our compiler will return a parse ERROR.
       To support it, we should parse an expression with two binary operators "*" and compile this expression to do the power-of computation.
    3) x = 1
       print(-x)
       Python will return -1, but our compiler will return a parse ERROR.
       To support it, we should add unary operators expression and deal with string argument correctly.

2. What resources did you find most helpful in completing the assignment?
    Ans:
    Yousef’s Tutorial and piazza discussion.

3. Who (if anyone) in the class did you work with on the assignment? (See collaboration below)
    Ans:
    No one. I worked on this assignment individually.