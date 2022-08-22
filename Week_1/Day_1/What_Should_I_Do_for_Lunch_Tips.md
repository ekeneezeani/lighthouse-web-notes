### Tips

Try experimenting with the comparison operators (`<`, `>`, `===`, etc.) in the node REPL, which you can launch using the `node` command in Vagrant.

Work on your code iteratively – that means in small pieces. 

To help you figure out how to use `hungry` and `availableTime` inside your function, try outputting their values to the Terminal as follows.

``` javascript
const whatToDoForLunch = function(hungry, availableTime) {
  if (hungry === true) {
    if  (availableTime < 20) {
      console.log("I'm hungry and I have " + availableTime + " minutes for lunch.");
      console.log('Pick up a snack or grab something you have ready at home');
      
    } else if (availableTime >= 20 && availableTime <= 30) {
      console.log("I'm hungry and I have " + availableTime + " minutes for lunch.");
      console.log('You deserve a break and should take time to cook a delicious meal');
      
    } else if (availableTime > 30) {
      console.log("I'm hungry and I have " + availableTime + " minutes for lunch.");
      console.log('It is an intense program, you should reconsider taking too much time on');
      
    }
  } else {
    console.log("I'm not hungry and I have " + availableTime + " minutes for lunch.");
  }
};

/*
 * This is some test runner code that's simply calling our whatToDoForLunch function
 * defined above to verify we're making the right decisions. Do not modify it!
 */


whatToDoForLunch(true, 20);
whatToDoForLunch(true, 50);
whatToDoForLunch(false, 30);
whatToDoForLunch(true, 15);