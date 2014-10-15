#ReadMe.md
###What is it?
Radon JS is my Javascript Framework for building 2d canvas games in Javascript. The framework provides the user with a series of simple functions for building fantastic games in no time. The framework is designed for hobbyists and beginers.
===
##Documentation
Welcome to the documentation for my Javascript Game Framework.
###Getting Started

Radon has two main functions, the setup function and the draw function. The setup function is the first function called when your game begins, it is only called once in a game cycle. Within the setup function you should initiate all the starting variables for your game and do calculations you will only need to do once per game.

As you can see in the example below in this setup function the background for the canvas is set to red and the varibles for the initial positioning of the sprite are set up.
```javascript
function setup() {
  background("red");
  shape2 = {
        x: 50,
        y: 10,
        width: 10,
        height: 10,
        color: "black",
    };
}
```

The second function is the draw function, this function is called approxiametely 33 times per second. In this function you should manipulate your x and y values to move your characters, check for collisions and work with user input.

For example in the draw function below the x position of shape 1 is set to the mouse position and shape 1 is then redrawn at its new x coardinate.
```javascript
function draw() {
  shape1.x = mousePos.x;
  fillRect(shape1.x, shape1.y, shape1.width, shape1.height, shape1.color);
}
```
> Blockquotes are very handy in email to emulate reply text.
> This line is part of the same quote.

___

###Graphics
___
**Drawing Squares**
```javascript
fillRect(x, y, width, height, color)
```
> Blockquotes are very handy in email to emulate reply text.
> This line is part of the same quote.

###Game Logic
___
###User Input
___
###Data Handling
___
