<h1>
  <span class="headline">JavaScript Control Flow</span>
  <span class="subhead">Truthy and Falsy</span>
</h1>

**Learning objective:** By the end of this lesson, you will be able to predict whether a value makes an `if` statement run.

## Conditions do not need to be Booleans

You have seen comparisons such as `5 > 3`, which produce `true`.

But an `if` condition can be **any expression that produces a value**. JavaScript checks that value as though it were `true` or `false`.

- **Truthy:** JavaScript treats the value as `true` for the condition.
- **Falsy:** JavaScript treats the value as `false` for the condition.

The original value does **not** change into a Boolean.

```js
if ('Hello') {
  console.log('This runs')
}
```

`'Hello'` is a non-empty string, so it is truthy.

## Common falsy values

For now, remember these values:

| Value | What it means |
| --- | --- |
| `false` | Boolean false |
| `0` | The number zero |
| `''` or `""` | An empty string |
| `null` | No value |
| `undefined` | A value has not been assigned |
| `NaN` | A number calculation did not produce a valid number |

Most other values are truthy. For example, `1`, `-5`, `'0'`, `'false'`, and `' '` (one space) are all truthy.

> 🧠 An empty array `[]` and an empty object `{}` are **truthy** even though they are empty. Don't use `if (myArray)` to check if an array has items.

## Try it in code

```js
const customerName = 'Aisha'

if (customerName) {
  console.log(`Welcome, ${customerName}`)
} else {
  console.log('Please enter your name')
}
```

Change `customerName` to `''` and run it again. The `else` block will run.


## 🎓 You Do

Before running each condition, predict whether it logs `'Runs'`.

```js
if (0) { console.log('Runs') }
if ('0') { console.log('Runs') }
if ([]) { console.log('Runs') }
if ('') { console.log('Runs') }
if (10 > 3) { console.log('Runs') }
```

Then test your answers with `node app.js`.

> 🧠 Curly braces help show which code belongs to each condition.
