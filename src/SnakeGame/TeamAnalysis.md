# Group Members' Names: Sonal Sekhda, Akira, Kevin, and  Joseph

# SimpleSnakeGame:
Snake game is about how to create a game in java and is also about a snake gets longer when it eats an apple.

## Initialization and main method:
Main method runs a program. In main method, Constructor called JFrame created for the window.
After that the constructor name SimpleSnakeGame created.
In JFrame object variable gamePanel added, so it appears inside the main window.
setDefaultCloseOperation that closes the window when game ends.
setTitle that sets title " Simple Snake Game"
setResizeable set at false, so it does not change size and with 
setLocationRelativeTo that window stays in the center. 
pack()method with JFrame object resize the window.
## Class variables:
SIZE, UNIT_SIZE, GAME_UNITS, DELAY, and keyEvent

## SimpleSnakeGame constructor:
SimpleSnakeGame is Constructor and gives the size, background color, boolean value true for focus 
and added KeyListener with new method.
there is call method start game.

## startGame method:
call method newApple, instance variable running set at true;
timer set to delay start, and timer object with start method 
## newApple method:
new apple value set at x any y co-ordinate with math random number.

## paintComponent method:
super means calling a SimpleSnakeGame with variable g.
draw method with graphic g variable.

## draw method:
There is if Condition, boolean running  false then drawLine with graphics for apple until condition match.
color set red and fillOval with variable appleX, appleY, UNIT_SIZE, and UNIT_SIZE. Same way for the  snake.
if condition does not match the game will be over.
## move method:
in move method snake's body moves in right direction because direction variable specified. 
in the for loop snake moves forward so its start from end of the body and reaches to the head of the snake.

## checkApple method:
if condition to check that if snake ear apple or not. if snake eats then body will grow by one block.
and keeps track that many number of apple eaten. 
After the apple eaten it goes to newApple method and new apple will appear in different position. 
## checkCollisions method:
if the snake collide with left, right, upper, or lower border then game will be over.
## gameOver method:
When game ends, the message set to appear with Red color, Font bold and size 30.
and for the fonts there is method to getFontMetrics. 
and message appears "Game Over"
## actionPerformed method:
Checks condition, if running then that goes to move method, next goes checkApple method, 
and then checkCollisions method.
## MyKeyAdapter class:
 Checks the Key pressing activity by checking condition with Switch.