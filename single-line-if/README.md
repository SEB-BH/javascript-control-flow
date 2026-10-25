<h1>
  <span class="headline">JavaScript Control Flow</span>
  <span class="subhead">Single Line <code>if</code></span>
</h1>

**Learning objective:** By the end of this lesson, you will be able to read a one-line `if` statement and rewrite it with curly braces.

## One-line `if` statements

You may see an `if` statement written without curly braces:

```js
const stock = 3

if (stock > 0) console.log('In stock')
```

This is valid JavaScript. When there are no curly braces, only the **next statement** belongs to the `if`.

It does the same thing as:

```js
const stock = 3

if (stock > 0) {
  console.log('In stock')
}
```

## Which should you use?

**Use curly braces in your own code.** They make it easier to see which lines belong to the condition, especially as your program grows.

## 🎓 You Do

Rewrite this example using curly braces:

```js
const score = 10

if (score >= 10) console.log('Level complete')
```

Make sure it prints the same message.
