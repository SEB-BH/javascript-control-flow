<h1>
  <span class="headline">JavaScript Control Flow</span>
  <span class="subhead">Branching</span>
</h1>

**Learning objective:** By the end of this lesson, you will be able to use `if`, `else`, and `else if` to make decisions in JavaScript.

## What goes inside an `if` statement?

An `if` statement checks a **condition** and runs code when that condition is **truthy**.

```js
if (true) {
  console.log('The condition is truthy')
}
```

The condition can be **any expression that produces a value**. JavaScript checks whether that value is truthy or falsy. A comparison is one common way to produce `true` or `false`.

```js
const stock = 5

console.log(stock > 0) // true

if (stock > 0) {
  console.log('In stock')
}
```

Here, `stock > 0` evaluates to `true`, so the message appears.

> 💡 The parentheses `()` hold the condition. The curly braces `{}` hold the code to run.

You can also use a Boolean variable directly:

```js
const isLoggedIn = true

if (isLoggedIn) {
  console.log('Welcome back!')
}
```

Or even a value that is not a Boolean:

```js
if ('Bahrain') {
  console.log('This runs')
}
```

A non-empty string is **truthy**, so this code runs. We will explore truthy and falsy values in a later lesson.

## `if`: one possible path

If the condition is falsy, JavaScript **skips** the block.

```js
const stock = 0

if (stock > 0) {
  console.log('In stock')
}

console.log('Stock check complete')
```

Only `Stock check complete` is printed.

## `if...else`: two paths

Use `else` when you want something to happen if the condition is falsy.

```js
const stock = 0

if (stock > 0) {
  console.log('In stock')
} else {
  console.log('Sold out')
}
```

Exactly one of the two blocks runs.

## `if...else if...else`: three or more paths

Use `else if` to check another condition. JavaScript checks from top to bottom and runs the **first matching block**.

```js
const deliveryStatus = 'shipped'

if (deliveryStatus === 'delivered') {
  console.log('Your order has arrived')
} else if (deliveryStatus === 'shipped') {
  console.log('Your order is on the way')
} else if (deliveryStatus === 'processing') {
  console.log('We are preparing your order')
} else {
  console.log('Unknown status')
}
```

## 🎓 You Do

Create a variable called `color`, then write an `if...else if...else` statement:

- `'green'` → log `'Go'`
- `'yellow'` → log `'Slow'`
- `'red'` → log `'Stop'`
- Anything else → log `'Unknown color'`

Change the value of `color` to test **all four results**.

> 🧠 After writing a condition, ask: *What happens when it is true? What happens when it is false?*
