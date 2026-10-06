# Programming Languages — Course Notes

LaTeX notes for CSCI-GA 2110 (Programming Languages), NYU Courant, Fall 2026, taught by Prof. Joseph Tassarotti (recitations: Seong-Heon Jung, Vishnu Satish). Notes by You Li.

One chapter per week: the lecture, split into one section per topic, followed by that week's recitation. Recitation solutions follow the TA's posted `*-solutions.rkt`. Sections marked (SUPPLEMENT) go beyond the course material, drawing on Krishnamurthi's *PLAI*, *HtDP*, *SICP*, and Pierce's *TAPL*.

## Layout

```
main.tex        title page, acknowledgements, notation, bibliography; includes the chapters
plnotes.sty     page layout, boxed definition/key-point/pitfall/exercise environments, Racket listings, figure styles
chapters/
  ch01-week1.tex          Week 1 (L1, R1): reading list, roadmap; inputs week1/
  week1/
    01-why-study.tex              classification vs. building blocks, interpreters vs. compilers, logistics
    02-expressions-recursion.tex  define, cond, recursion, tail recursion
    03-pairs-lists.tex            cons cells, lists, my-reverse
    04-recitation1.tex            traffic lights, specifications, scroll, all-even, tail-recursive reverse
  ch02-week2.tex          Week 2 (L2, R2)
  week2/
    01-lists-accumulators.tex     snoc, rev, rev-alt, sum-list, named let
    02-structs-trees.tex          struct, #:transparent, binary trees, match
    03-higher-order.tex           lambda, closures, map, filter, foldl/foldr
    04-scope-state.tex            let/let*, lexical scope, purity, begin, boxes
    05-recitation2.tex            bexp interpreter, De Morgan optimizer, testing an optimization
  ch03-week3.tex          Week 3 (L3, R3)
  week3/
    01-types.tex                  plai-typed types, inference, function types, pairs, polymorphism
    02-define-type.tex            define-type, type-case, exhaustiveness
    03-calculator.tex             quote, s-expressions, parse/eval for ArithE
    04-recitation3.tex            typed bexp, nested type-case, match patterns
  ch04-week4.tex          Week 4 (L4, R4)
  week4/
    01-let-subst.tex              idC/letC, eager substitution, shadowing
    02-lazy-capture.tex           lazy substitution, variable capture
    03-capture-avoiding.tex       gensym, typed-in, subst-lazy-v2
    04-lambda.tex                 lambdaC/appC, Value, eval-lazy-v2
    05-recitation4.tex            match in the interpreter (PatternE, parse-patterns, subst-pattern, get-pat-expr)
```

## Build

```
latexmk -pdf main.tex
```

The runnable scribble notes (`../lectures/lecN-notes.rkt`, `../recitation/recitationN-notes.rkt`) hold the same code with tests.
