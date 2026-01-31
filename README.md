# first-follow-grammar
A C program that displays FIRST and FOLLOW sets for a context free grammar used in Compiler Design and LL(1) parsing.This project is a Compiler Design utility that demonstrates how to compute and display FIRST and FOLLOW sets for a given grammar used in **LL(1) parsing**.
The grammar used in this program is:
## What are FIRST and FOLLOW?
### FIRST Set
FIRST(X) is the set of terminals that can appear at the beginning of strings derived from X.
### FOLLOW Set
FOLLOW(X) is the set of terminals that can appear immediately to the right of X in some sentential form.
These are essential for building:
- Predictive parsers
- LL(1) parsing tables

## Program Output
### Grammar
E → E + T | T
T → T * F | F
F → ( E ) | i
### FIRST Sets
FIRST(E) = { (, i }
FIRST(T) = { (, i }
FIRST(F) = { (, i }
### FOLLOW Sets
FOLLOW(E) = { $, +, ) }
FOLLOW(T) = { $, +, *, ) }
FOLLOW(F) = { $, +, *, ) }
