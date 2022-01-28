### Tips

Try experimenting with the comparison operators (`<`, `>`, `===`, etc.) in the node REPL, which you can launch using the `node` command in Vagrant.

Work on your code iteratively – that means in small pieces. 

To help you figure out how to use `hungry` and `availableTime` inside your function, try outputting their values to the Terminal as follows.

```javascript
const whatToDoForLunch = function (hungry, availableTime) {

  if (hungry === true && 30 < availableTime) {
    return "Wait~~!!!! we are in bootcamp and that we should reconsider how much time we actually have to spare.";
  }
  if (hungry === true && availableTime < 20) {
    return `we want to pick something up and eat it in the lab.`;
  }
  if (hungry === true && 20 <= availableTime <= 30) {
    return "We should try a place nearby.";
  } else {
    return `I'm not hungry and I have ${availableTime} minutes for lunch.`;
  }
};