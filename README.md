### Goal: Write your own “documentation” for the higher order functions
**Your documentation should include:**
- A description of the purpose (what and why)
- A description of the syntax
- An example
- An explanation of the example
- Any additional notes/details

---
Your documentation here: 

# Higher Order Functions

Definition: **Higher order functions** are functions that *receive* another function as a parameter or return a function as as return value. Higher-order functions allow us to be more flexible with _how_ we interact with our arguments.

```js
function runCallback(x, callback) {
  callback(x);
}

function printLoudly(x) {
  console.log(x + "!!!")
}

runCallback('hello', console.log) // In this invocation, we use console.log to interact with 'hello'
runCallback('hello', printLoudly) // In this invocation, we use printLoudly to interact with 'hello'
```

This example will first log the string `hello` to the console. `myHigherOrderFunction` uses the parameter `callback` to substitute `console.log`. `arg` substitutes `'hello'`. When we invoke `myHigherOrderFunction` we will `console.log("hello")`.
