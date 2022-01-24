# Turing Machines
- A Turing machine consists of an infinitely long strip of tape divided into squares. It has a read/write head that can read symbols from the tape, make decisions and write/delete symbols.
- A Finite State Machine specifies the task to be performed, including moving the head.
- A Turing machine mas have at least one state, known as a halting state or stop state that causes it to halt for some inputs.

### Transition Functions
- A **transition RULE** is expressed as 'input, output, direction' for example '0, 0, R'. 
- **Transition FUNCTIONS** are described below.
- The transition rules for any Turing machine can be expressed as a transition function $\delta$. The rules are written in the form:
> $\delta$(Current State, Input Symbol) = (Next State, Output Symbol, Movement) 
> E.g:
> $\delta$(S1, 0) = (S2, 1, L)

- A Turing machine can theoretically represent any computation: this is a Universal Turing Machine (U)
- Given a description \<M\> of a machine M, followed by the data D, it can execute calculations on the data in the same way machine M would.
- This idea was likely the breakthrough that led to the idea of a stored-program computer, in which both the program and its data are held in memory.
