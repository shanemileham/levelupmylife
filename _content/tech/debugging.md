---
title: Debugging
---

{% include toc %}

## Prevention
- Architecture - simple, unidirectional, modular, documented, immutable
- Tests - cover each function and behavior

## Tools
- Debugger
- Console
- Browser debugging tools and inspector

## Debugging strategies
- (Prevention steps - see above)
- **Learn** - Expand relevant knowledge about the pieces involved in the puzzle (test via rubber duck)
- **Simplify** - Scope the problem down
- **Target** - Find the piece of the puzzle with the most things depending on it
- **Test** - Create a hypothesis and test it

_In general, debugging can be done in the order above; however, some paths might be quicker to implement and their cost therefore is lower. At points where there are multiple options going forward, it is usually best to follow a method between these two functions:_
- f(n) = g(n) + h(n)	(A* - better for overall simpler code)
- f(n) = h(n)		(better for finishing something quickly, even if it is more complicated)
- ...where g(n) is path distance to solution so far, and h(n) is expected distance to solution
- (measured in time/steps)

## Hypothesis Testing
- Belief (expectation): `? E --> X`
- Experience (test): `E --> Y`
  - Action taken
  - Result
- New belief: `? E --> Z`

## Post-Debug
- Look for similar errors and write automated test to ensure the error will never happen again
