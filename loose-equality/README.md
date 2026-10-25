<h1>
  <span class="headline">JavaScript Control Flow</span>
  <span class="subhead">Loose Equality</span>
</h1>

**Learning objective:** By the end of this lesson, you will be able to explain why beginners should normally use `===` instead of `==`.

## Two ways to compare equality

JavaScript has two equality operators:

```js
console.log(3 === '3') // false
console.log(3 == '3')  // true
```

**Strict equality (`===`)** compares values without converting one type to another. A number and a string are different types, so `3 === '3'` is false.

**Loose equality (`==`)** sometimes converts values before comparing them. This can produce surprising results.

**Our rule: use `===`** for equality checks and `!==` for inequality checks.

## 🎓 You Do

Predict the results, then check them in Node.js:

```js
console.log(5 === 5)
console.log(5 === '5')
console.log(5 !== '5')
```

📖 [MDN: Equality](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Equality)
