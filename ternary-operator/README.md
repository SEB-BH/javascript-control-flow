<h1>
  <span class="headline">JavaScript Control Flow</span>
  <span class="subhead">Ternary Operator</span>
</h1>

**Learning objective:** By the end of this lesson, you will be able to use a ternary operator to choose between two values.

## A short way to choose a value

First, look at a normal `if...else` statement:

```js
const stock = 4
let message

if (stock > 0) {
  message = 'In stock'
} else {
  message = 'Sold out'
}

console.log(message)
```

A **ternary operator** can choose the same value in one line:

```js
const stock = 4
const message = stock > 0 ? 'In stock' : 'Sold out'

console.log(message)
```

Read it like this:

```text
condition ? value if truthy : value if falsy
```

The `?` comes after the condition. The `:` separates the two possible values.

## When should you use it?

Use a ternary for a **simple choice between two values**. For longer decisions or several actions, use `if...else` instead.

## 🎓 You Do

Create a variable called `orderTotal`. Use a ternary operator to store one of these strings in `deliveryMessage`:

- If `orderTotal >= 10`, use `'Delivery available'`.
- Otherwise, use `'Add more items for delivery'`.

Log the message, then try a different total.

📖 [MDN: Conditional (ternary) operator](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Conditional_operator)
