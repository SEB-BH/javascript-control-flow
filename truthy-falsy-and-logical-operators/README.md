<h1>
  <span class="headline">JavaScript Control Flow</span>
  <span class="subhead">Truthy, Falsy, and Logical Operators</span>
</h1>

**Learning objective:** By the end of this lesson, you will be able to recognize when `||` and `&&` return a value instead of a Boolean.

## Logical operators can return other values

You have used `||` (OR) and `&&` (AND) with Boolean conditions.

They can also be used with strings, numbers, and other values.

### `||` returns the first truthy value

```js
console.log('Aisha' || 'Guest') // 'Aisha'
console.log('' || 'Guest')      // 'Guest'
```

This can provide a simple default name:

```js
const enteredName = ''
const displayName = enteredName || 'Guest'

console.log(displayName) // 'Guest'
```

If both values are falsy, `||` returns the last one.

### `&&` returns the first falsy value (or the last value)

```js
console.log(0 && 'Ready')    // 0
console.log(true && 'Ready') // 'Ready'
```

`&&` only reaches the second value when the first is truthy.

## Keep conditions easy to read

You may see shortcuts like this:

```js
const isLoggedIn = true
isLoggedIn && console.log('Welcome back')
```

For now, prefer a regular `if` statement. It makes the decision clearer:

```js
const isLoggedIn = true

if (isLoggedIn) {
  console.log('Welcome back')
}
```

## 🎓 You Do

Predict the results, then run the code:

```js
console.log(0 || 15)
console.log('Bahrain' || 'Guest')
console.log('' && 'Hello')
console.log(5 && 'Complete')
```

> 🧠 This is optional knowledge. For most beginner exercises, use `if` statements and compare values directly.
