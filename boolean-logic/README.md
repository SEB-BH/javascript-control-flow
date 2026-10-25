<h1>
  <span class="headline">JavaScript Control Flow</span>
  <span class="subhead">Boolean Logic</span>
</h1>

**Learning objective:** By the end of this lesson, you will be able to compare values and combine conditions.

## What is a Boolean?

A **Boolean** is either `true` or `false`.

```js
console.log(10 > 5)  // true
console.log(10 < 5)  // false
```

In JavaScript, an **expression** is code that produces a value. For example, `10 > 5` is an expression. Its value is `true`.

An **operator** is a symbol that does a job, such as `>` or `===`.

## Comparison Operators

| Operator | Meaning | Example | Result |
| --- | --- | --- | --- |
| `===` | Equal to (same value and type) | `3 === 3` | `true` |
| `!==` | Not equal to | `3 !== 4` | `true` |
| `>` | Greater than | `8 > 5` | `true` |
| `<` | Less than | `8 < 5` | `false` |
| `>=` | Greater than or equal to | `5 >= 5` | `true` |
| `<=` | Less than or equal to | `4 <= 5` | `true` |

Try these in `app.js`:

```js
const productPrice = 15
const budget = 20

console.log(productPrice <= budget) // true
console.log(productPrice === 20)    // false
```

> 🧠 Use `===` to check equality. Do not confuse it with `=`: one equals sign **assigns** a value to a variable.

## Combine conditions with Logical Operators

Sometimes we need to check **two conditions**.

**AND (`&&`)** requires both conditions to be true.

```js
const hasTicket = true
const isEventOpen = true

console.log(hasTicket && isEventOpen) // true
```

**OR (`||`)** requires at least one condition to be true.

```js
const isStudent = false
const hasDiscountCode = true

console.log(isStudent || hasDiscountCode) // true
```

**NOT (`!`)** changes a Boolean to its opposite.

```js
const isClosed = false

console.log(!isClosed) // true
```

### Combining logical operators with comparisons

We can also combine logical operators with comparison operators.

For example, imagine a store that only gives discounts to customers who are at least 18 years old AND have a membership.

```js
const age = 22
const hasMembership = true

console.log(age >= 18 && hasMembership) // true
```

## 🎓 You Do

Create these variables:

```js
const orderTotal = 12
const minimumForDelivery = 10
const hasAddress = true
```

1. Log whether `orderTotal` is at least `minimumForDelivery`.
2. Log whether the customer has an address **and** qualifies for delivery.
3. Change `orderTotal` to `8` and run the file again. What changes?
