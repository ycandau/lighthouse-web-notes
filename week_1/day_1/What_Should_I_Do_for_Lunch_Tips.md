### Tips

Try experimenting with the comparison operators (`<`, `>`, `===`, etc.) in the node REPL, which you can launch using the `node` command in Vagrant.

Work on your code iteratively – that means in small pieces.

To help you figure out how to use `hungry` and `availableTime` inside your function, try outputting their values to the Terminal as follows.

```javascript
function whatToDoForLunch(hungry, availableTime) {
  console.log('hungry is', hungry);
  console.log('availableTime is', availableTime);
}
```

---

### Completed code

Using ternary operators for more conciseness.

```javascript
const whatToDoForLunch = function (hungry, availableTime) {
  const msg = !hungry
    ? 'Get back to work!'
    : availableTime < 20
    ? "Let's pick something up and eat in the lab."
    : availableTime <= 30
    ? "Let's try a place nearby."
    : "Let's reconsider... This is bootcamp after all!";
  console.log(msg);
};
```
