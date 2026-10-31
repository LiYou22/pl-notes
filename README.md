# Programming Languages Notes

LaTeX notes for CSCI-GA 2110 (Programming Languages), NYU Courant, Fall 2026, Prof. Joseph Tassarotti (recitations by Seong-Heon Jung and Vishnu Satish). The compiled notes are in `pl-notes.pdf`.

## Chapters

One chapter per week; each ends with that week's recitation.

1. **Course Introduction and Racket Basics**: why study programming languages, interpreters vs. compilers, `define` and `cond`, recursion and tail recursion, pairs and lists.
2. **Higher-Order Functions, Scope, and State**: accumulators, structs and trees, `lambda` and closures, `map`/`filter`/`fold`, `let` and `let*`, lexical scope, boxes.
3. **Types and a First Interpreter**: types in `plai-typed`, `define-type` and `type-case`, parsing and evaluating a calculator.
4. **Names and Functions**: `let` and substitution, variable capture, capture-avoiding substitution, adding functions.
5. **From Substitution to Environments**: lambda calculus and alpha equivalence, environment interpreters, dynamic vs. lexical scope, closures.
6. **Mutable State**: boxes, store passing, environment vs. store, meta-circular interpreters.
7. **Recursion and Objects**: why `let` cannot recurse, cyclic data and backpatching, `fix` and the Y/Z combinators, objects as closures.
8. **Macros**: `syntax-case` and `define-syntax-rule`, `while` and `or` as macros, ellipses, hygiene, literal keywords, anaphoric `if`.
