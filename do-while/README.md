<h1>
  <span class="headline">JavaScript Control Flow</span>
  <span class="subhead"><code>do...while</code></span>
</h1>

**Learning objective:** By the end of this lesson, you will be able to explain why a `do...while` loop always runs at least once.

## Run first, check second

A `while` loop checks its condition **before** it runs the code.

A **`do...while` loop** runs the code **once before** it checks the condition.

```js
let number = 10

do {
  console.log(number)
  number++
} while (number < 5)
```

The output is `10`. The condition is already false, but the code runs once before JavaScript checks it.

> 💡 You will use `for` loops more often in this part of the course. The important difference to remember is that `do...while` always runs at least once.

## 🎓 You Do

Change the starting number to `1` and predict the output. Run the code to check your answer.
