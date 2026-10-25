<h1>
  <span class="headline">JavaScript Control Flow</span>
  <span class="subhead">Instructor Guide</span>
</h1>

## Teaching focus

Teach the **core lessons first**. Students should finish knowing how to compare values, write `if...else` statements, and use `for` loops. The remaining folders are optional and stay in their original locations.

**Key sentence to repeat:** *The condition of an `if` statement can be any expression that produces a value. JavaScript checks whether the result is truthy or falsy.*

Avoid teaching `==` as an alternative to `===`. Students should use `===` and `!==` for comparisons.

## Core lessons

| Lesson | Skills |
| --- | --- |
| [Setup](../setup/README.md) | Run `app.js` with Node.js |
| [Concepts](../concepts/README.md) | Sequence, branching, and looping |
| [Boolean Logic](../boolean-logic/README.md) | Comparisons and simple logical operators |
| [Branching](../branching/README.md) | `if`, `else if`, and `else` |
| [Looping](../looping/README.md) | Counting with a `for` loop |
| [Truthy and Falsy](../truthy-and-falsy/README.md) | Checking the result of any expression |

## Level up lessons

| Lesson | Skills |
| --- | --- |
| [Single Line `if`](../single-line-if/README.md) | Read one-line `if` statements |
| [Nested Statements](../nested-branching-statements/README.md) | Check one condition inside another |
| [Ternary Operator](../ternary-operator/README.md) | Choose between two values |
| [`switch` Statement](../switch-statements/README.md) | Check several cases |
| [`while`](../while/README.md) | Repeat until a condition changes |
| [`do...while`](../do-while/README.md) | Run before checking the condition |
| [Loose Equality](../loose-equality/README.md) | Recognize `==` but prefer `===` |
| [Truthy, Falsy, and Logical Operators](../truthy-falsy-and-logical-operators/README.md) | Explore non-Boolean results from `||` and `&&` |

## Common beginner misunderstandings

- `=` assigns a value; `===` compares values.
- `if (value)` is allowed; the condition does not have to be a comparison.
- `if ([])` is truthy; use `.length` to check for items.
- A `for` loop stops only when its condition becomes falsy.
- In an `if...else if` chain, JavaScript executes the first matching branch.

## Quick checks

Ask students to predict the console output before running each example. Then let them change one value and run it again. This helps them connect the condition to the output.

## References

📖 [Reference Materials](../references/README.md)

## Internal

### Prerequisites

- Intro to JavaScript

### Course landing pages

- [Default Landing Page](https://ga-curriculum.github.io/javascript-control-flow/canvas-landing-pages/fallback)
- [SEB - Software Engineering Bootcamp](https://ga-curriculum.github.io/javascript-control-flow/canvas-landing-pages/seb)

### Resources

🎥 [Video Hub](./video-hub.md)

🏗️ [Release Notes](./release-notes.md)
