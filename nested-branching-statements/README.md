<h1>
  <span class="headline">JavaScript Control Flow</span>
  <span class="subhead">Nested Branching Statements</span>
</h1>

**Learning objective:** By the end of this lesson, you will be able to read and write an `if` statement inside another `if` statement.

## One decision inside another

Sometimes you need to check a second condition **only after** the first one is true. This is called a **nested `if` statement**.

For example, a user must first be logged in, then they must have permission to edit:

```js
const isLoggedIn = true
const canEdit = false

if (isLoggedIn) {
  console.log('User is logged in')

  if (canEdit) {
    console.log('Show the Edit button')
  } else {
    console.log('Editing is not allowed')
  }
} else {
  console.log('Please sign in')
}
```

The inner `if` runs **only if** `isLoggedIn` is truthy.

## Keep it readable

Nested code is useful, but too many levels can be hard to follow. Sometimes `&&` is simpler:

```js
const isLoggedIn = true
const canEdit = false

if (isLoggedIn && canEdit) {
  console.log('Show the Edit button')
}
```

Use the version that makes the decision easiest to understand.

## 🎓 You Do

Create two variables: `hasAccount` and `hasVerifiedEmail`.

- If `hasAccount` is false, log `'Create an account'`.
- If `hasAccount` is true but `hasVerifiedEmail` is false, log `'Verify your email'`.
- If both are true, log `'You can continue'`.

Change the variables to test all three paths.
