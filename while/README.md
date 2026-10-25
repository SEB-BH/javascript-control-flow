<h1>
  <span class="headline">JavaScript Control Flow</span>
  <span class="subhead"><code>while</code></span>
</h1>

**Learning objective:** By the end of this lesson, you will be able to write a `while` loop that stops when its condition becomes falsy.

## Repeat while a condition is true

A **`while` loop** checks a condition before every repeat.

```js
let itemsPacked = 0

while (itemsPacked < 3) {
  itemsPacked++
  console.log(`Packed: ${itemsPacked}`)
}
```

Output:

```text
Packed: 1
Packed: 2
Packed: 3
```

The loop checks `itemsPacked < 3`. As soon as that becomes false, it stops.

## `for` or `while`?

- Use a **`for` loop** when you are counting through a known range (such as 1 to 10).
- Use a **`while` loop** when you want to repeat until a condition changes.

Both can repeat code. Choose the one that is easier to read.

## Watch out for infinite loops

This loop never updates its counter, so it will not stop:

```js
// Do not run this example!
// let itemsPacked = 0
// while (itemsPacked < 3) {
//   console.log('Packing...')
// }
```

> 🧠 Always ask: *What will change so the condition eventually becomes falsy?*

## 🎓 You Do

Start with `let remainingTasks = 4`. Use a `while` loop to print the number of remaining tasks, then reduce it by 1 each time. Stop when there are no tasks left.
