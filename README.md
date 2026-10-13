# Programming Languages Notes

My LaTeX notes for CSCI-GA 2110 (Programming Languages) at NYU Courant, Fall 2026. Prof. Joseph Tassarotti teaches the lectures; Seong-Heon Jung and Vishnu Satish run the recitations.

I organize them by week. Each chapter covers that week's lecture, split into sections by topic, and ends with the recitation. For recitation problems I follow the TA's posted solutions (`*-solutions.rkt`) rather than my own attempts.

## Files

```
main.tex        title page, notation, bibliography
plnotes.sty     layout, the boxed environments, Racket listings, figure styles
chapters/
  ch01-week1.tex          Week 1 (sections are in week1/)
  week1/
    01-why-study.tex              why study PLs, interpreters vs. compilers, logistics
    02-expressions-recursion.tex  define, cond, recursion, tail recursion
    03-pairs-lists.tex            cons cells and lists
    04-recitation1.tex            Recitation 1
  ch02-week2.tex          Week 2
  week2/
    01-lists-accumulators.tex     more list functions, accumulators, named let
    02-structs-trees.tex          structs, binary trees, match
    03-higher-order.tex           lambda, closures, map/filter/fold
    04-scope-state.tex            let and let*, lexical scope, mutation and boxes
    05-recitation2.tex            Recitation 2: a boolean-expression interpreter, De Morgan
  ch03-week3.tex          Week 3
  week3/
    01-types.tex                  types in plai-typed
    02-define-type.tex            define-type and type-case
    03-calculator.tex             s-expressions, parse and eval for the calculator
    04-recitation3.tex            Recitation 3: the typed version, match patterns
  ch04-week4.tex          Week 4
  week4/
    01-let-subst.tex              let, eager substitution, shadowing
    02-lazy-capture.tex           lazy substitution, variable capture
    03-capture-avoiding.tex       capture-avoiding substitution with gensym
    04-lambda.tex                 adding functions
    05-recitation4.tex            Recitation 4: adding match to the interpreter
  ch05-week5.tex          Week 5
  week5/
    01-subst-revisited.tex        let as application, capture, lambda calculus, alpha equivalence
    02-environments.tex           an environment interpreter for let (lecture5a)
    03-dynamic-scope.tex          lazy let with environments, dynamic vs. lexical scope (5b, 5c)
    04-closures.tex               lambda with environments, closures (5d, 5e)
    05-recitation5.tex            Recitation 5: environments as functions, static vs. dynamic, macros
  ch06-week6.tex          Week 6
  week6/
    01-state-boxes.tex            box, unbox, set-box!, begin; a first attempt that cannot mutate
    02-store-passing.tex          locations, the store, threading it through eval
    03-store-boxes.tex            the box clauses, traces of ex4 and ex5, env vs. store
    04-meta-circular.tex          boxes and functions implemented with Racket's; what each version explains
    05-recitation6.tex            Recitation 6 (placeholder)
```

## Building

```
latexmk -pdf main.tex
```

For a new week, add `chapters/chNN-weekN.tex` with a `weekN/` folder next to it, and `\include` it in `main.tex`.

The lecture code is in `../lectures/`. Recitations 3 and 4 also have runnable scribble notes with tests in `../recitation/`.
