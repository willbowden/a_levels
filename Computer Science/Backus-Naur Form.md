# Backus-Naur Form
> A meta-language is a language that describes another language.
> It lays out the rules for the syntax of the language.
> Backus-Naur form is one such meta-language.
> Many constructs that could be written using a regular expression can be written more succinctly using BNF.
> **Backus-Naur form is useful for computers because it is unambiguous (computer languages cannot be ambiguous) and can express languages that cannot be done with RegEx.**

### Structure
BNF is composed as a list of statements in the form:
> \<element\> ::= RULES
> | means OR

For example:
\<upper\> ::= A|B|C....
\<digit\> ::= 0|1|2|3|4|5|6|7|8|9
\<variable name\> \<letter\>|\<letter\>\<digit\>

### Recursive Rules
BNF often makes use of recursion where a statement is defined in terms of itself. E.g:
> \<variable list\> ::= \<variable\>|\<variable\>\<variable list\>

- The process of ascertaining whether a given statement is valid using the BNF definition is called parsing.
- It is done by reading left to write and replacing meta-variables with more comprehensive meta-variables at each stage.

### Syntax Diagrams
Syntax diagrams are a graphical method of representing the syntax of a language and map directly to BNF.

| Shape                                  | Meaning                                                                |
| -------------------------------------- | ---------------------------------------------------------------------- |
| ![[Terminal Element.png]]              | Terminal element (cannot be further broken down)                       |
| ![[Non-Terminal Element.png]]          | Non-terminal element, which will be defined in another syntax diagram. |
| ![[Repeated Non-Terminal Element.png]] | Non-terminal element that may be used more than once.                  |

Syntax diagrams start with a regular line leading into the diagram, and arrows connecting elements to following ones, until the end where a final arrow depicts the syntax being accepted.