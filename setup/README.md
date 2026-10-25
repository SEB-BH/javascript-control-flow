<h1>
  <span class="headline">JavaScript Control Flow</span>
  <span class="subhead">Setup</span>
</h1>

**Learning objective:** By the end of this lesson, you will be able to run a JavaScript file with Node.js.

We will write JavaScript in `app.js` and see the results in the terminal. You do not need an HTML file for this lesson.

## Create the project

Open **Git Bash** (Windows) or **Terminal** (Mac). Make a folder for your work:

```bash
mkdir -p ~/code/ga/lectures
cd ~/code/ga/lectures
mkdir javascript-control-flow
cd javascript-control-flow
touch app.js
code .
```

> 💡 If you already have a `lectures` folder, you can use it. If `code .` does not work, open the `javascript-control-flow` folder in VS Code yourself.

## Check your setup

In `app.js`, add:

```js
console.log('JavaScript is working!')
```

Save the file. In the VS Code terminal, run:

```bash
node app.js
```

You should see:

```text
JavaScript is working!
```

Every time you change your code, **save the file and run `node app.js` again**.

> 🧠 If the terminal says `node: command not found` or `node is not recognized`, ask an instructor to help you check your Node.js installation.
