<h1>
  <span class="headline">JavaScript Control Flow</span>
  <span class="subhead"><code>switch</code> Statements</span>
</h1>

**Learning objective:** By the end of this lesson, you will be able to read a `switch` statement and use it to check one value against several choices.

## Another way to check several options

A `switch` statement can be useful when you are comparing **one value** to several possible values.

You already know how to write this with `if...else if`:

```js
const orderStatus = 'shipped'

if (orderStatus === 'pending') {
  console.log('Order received')
} else if (orderStatus === 'shipped') {
  console.log('On the way')
} else {
  console.log('Unknown status')
}
```

Here is the same decision with `switch`:

```js
const orderStatus = 'shipped'

switch (orderStatus) {
  case 'pending':
    console.log('Order received')
    break
  case 'shipped':
    console.log('On the way')
    break
  default:
    console.log('Unknown status')
}
```

- `switch (orderStatus)` selects the value to check.
- Each `case` is a possible match.
- `break` stops JavaScript from continuing into the next case.
- `default` handles values that do not match any case.

> 💡 If you leave out `break`, JavaScript continues into the next case. For now, include `break` after each case's code unless you have a specific reason not to.

## 🎓 You Do

Create `const department = 'sales'`. Write a `switch` statement:

- `'sales'` → `'Contact the sales team'`
- `'support'` → `'Contact customer support'`
- Anything else → `'Department not found'`

Change `department` to test every path.

📖 [MDN: `switch`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/switch)
