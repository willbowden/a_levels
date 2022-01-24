# Reverse Polish Notation
Normal mathematical expressions are written in a form called infix.
> Reverse Polish (also called postfix) is a notation of writing arithmetic expressions that is very well suited to computers.

- It eliminates the need for brackets in sub expressions.
- It produces expressions in a form suitable for evaluation using a stack.
- It is used in interpreters based on a stack, for example Postscript and bytecode.

In reverse polish notation, the operator follows the operands.

### Precedence Rules
From highest to lowest 

| Symbol | Meaning                        |
| ------ | ------------------------------ |
| ~      | Unary minus (negative numbers) |
| ^      | Exponentiation                 |
| * /    | Multiply and divide            |
| + - )  |                                |
| (      |                                |
| =      |                                |

### Form
An infix expression written as (6 * 7 ) + 4 would be written in postfix as:
> 6 7 * 4 +

This means: 
"Get 6 and 7, then multiply them together."
"Get 4, then add it to the result of the previous operation."

### Translating Infix --> Reverse Polish
Starting from the left hand side, allocate numbers to the operators and operands as follows:
- If the next symbol is an operand, allocate the next number to it. If it is an operator, move to the next operand.
- Ignore parentheses except in so far as they affect the order of calculation.
- Bearing in mind the rules of precedence, decide which is the next operation that should be performed, and as soon as its operands have been allocated numbers, back up and allocate it the next number.

E.g:
>a + b * c
>1---2--3
>1-5-2-4-3
>a b c \* +

### Translating Reverse Polish --> Infix
Scan left to right, writing down operands until you find two operands followed by an operator. Write down the unpaired operand, followed by the next two operands in a set of brackets, separated by the operator. Continue writing down operands until you find the next operator, which will operate on the two preceding operands.
E.g:
>25 16 18 + \* 12 -
>25 (16 + 18)
>25 \* (16 + 18)
>25 \* (16 + 18) - 12

### Evaluating RPN Using A Stack
A compiler can translate an infix expression into RPN, where it can then be evaluated by a computer using a stack:
- If the next token is an operand, place it on the stack.
- If the next token is an operator, remove the required number of operators from the stack, perform the operation, and put the result on the stack.

### Binary Expression Trees
- A binary tree can be constructed to represent an infix expression, by splitting the tree at the central operator, and then splitting from then on until the leaves are operands. 
- In-order traversal of the tree will give the infix expression.
- Post-order traversal will give the postfix/RPN expression.
E.g: 3 + ((5 + 9) * 2)
![[Binary Expression Tree.png]]