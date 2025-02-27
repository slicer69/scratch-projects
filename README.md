# Beginner Scratch Projects

This repository contains a collection of small Scratch projects and games.

I recently took on learning how to use Scratch (specifically Scratch 3) in order
to teach beginners about simple coding processes and making their own small games.
Scratch is a free coding development environment and community aimed at children and
people looking to learn how to put together programs. It is developed and maintained
by [https://scratch.mit.edu/] MIT.

Each Scratch project is contained in a portable SB3 file. An SB3 file can be loaded
into the Scratch 3 application and run. SB3 files are Zip files which contain the
code and images required to run them.

This repository contains the following demo programs and small games. Generally
speaking, the games listed below start out simple and get increasingly complex
the farther down the list one goes. If you are downloading this repository in
order to learn by example, I'd suggest starting with the first demo (Bouncing Ball)
and working your way down the list.


## Bouncing Ball (bouncing-ball.sb3)

This is a simple demo showing how images can be made to move around the screen
on their own. The demo begins with one ball bouncing and then clones itself so
there are two balls moving around. The balls gradually change colour and divide
until there are ten balls bouncing around the screen.

This demo demonstrates edge detection, colour changing, and cloning objects.

There is no input and no game elements. This is basically a screensaver.


## Catching (catching.sb3)

In this game an apple falls from the sky. The player uses the mouse pointer to position
a bowl under the apple. The player's goal is to catch the apple in the bowl before it hits
the ground. After the apple is caught or hits the ground it falls from the top of the
screen again.

This game demonstrates touch detection, getting objects to talk, and making an object
follow the mouse pointer.


## Pew (pew.sb3)

This is a simple arcade game in which a shark swims across the top of the screen. The player
moves a spaceship with the mouse across the bottom of the screen. The player's goal is to
fire an arrow into the shark as it flies overhead.

The player controls the spaceship's position with the mouse and fires shots with the
spacebar.

This demo features making an object follow the mouse, keyboard input, detecting object
collision, generating random values (for the shark's speed), and keeping track of a score.


## Colour Pong (colour-pong.sb3)

This is a one (or two) player game which draws inspiration from the classic Breakout game.
On the left side of the screen is a game of Breakout with a ball, paddle, and bricks. The
player's job is to use the paddle to catch the ball and keep it bouncing back upward. When
the ball hits bricks, the bricks are destroyed. Once all bricks have been destroyed, the game
is won.

Whenever the ball hits a brick it increases in speed, making it harder to catch the ball
with the paddle.

On the right side of the screen is a spaceship which fires arrows upward at four buttons.
The first three buttons are red, green, and blue. Hitting any of these buttons with an
arrow changes the colour of the bouncing ball. Hitting the fourth, yellow button with an
arrow, causes the bouncing ball to slow down.

The bouncing ball only destroys a brick it touches if the ball is the same colour as the brick.

The paddle is controlled using the Left and Right arrow keys.
The spaceship follows the mouse pointer. The spaceship fires an arrow when the left
mouse button is pressed.

This game can be played as a one-player game, with one person controlling both the paddle
and the spaceship. However, it is designed to be a co-operative game played by two people - 
one controlling the paddle with the arrow keys and the second person moving the ship with 
the mouse.

This demo explores several concepts together: making objects follow the mouse, keyboard
input, cloning an object (bricks) multiple times, rate of fire control for arrows using 
variables, collision detection (ball, bricks, and buttons), tracking the number of objects
on the screen (bricks), changing the rate of movement (ball), transmitting signals
to multiple objects which will response differently, and determining whether to react
to a collison based on an object's properties (costume).



## Minecrab (minecrab.sb3)

This is an underwater adventure featuring a crab (the 
player), a fish which drops rocks, and a shark which drops bombs.

The crab runs around on the sandy bottom and can dig down into the blocks of sand, mud, 
and rock. The fish drops rocks (which turn into new blocks of dirt).
 
Meanwhile the shark occasionally passes overhead and drops bombs which destroy blocks 
the bombs hit. When the bombs explode, the crab can be injured if it is too close.

The crab can be controlled using the arrow keys Left and Right to run, Up to jump, and Down
to stop. The crab can also be controlled using the A and D keys to move left and right. 
The W key jumps and the S key stops the crab.

To dig, the crab moves to a block of dirt and the user clicks (with the mouse) on the block
they want removed.

The crab has health points (represented by hearts in the upper-left corner) which are
reduced when the crab is hit by an explosion. When the hearts are reduced to zero, the
game is over.

There are no points, but the general idea of the game is to survive as long as possible. The
player may also wish to amuse themselves by digging in certain patterns, dodging the bombs,
or designing their own "ideal crab home". It's a literal sandbox game.

This game was a way to explore a number of concepts and glue them together. There is
keyboard-driven movement for the crab and random movement for the fish. In fact, a lot
of this game is random - the appearances of the shark, where new rocks are dropped, and when
the fish and shark say something.

There is also object touching detection, mostly with things running into blocks (like the
crab, bombs, and rocks). Plus we need to test distance between the crab and fish as well
as see how close the crab is to blocks of dirt

Another recurring feature in the code are signals, which tell us when one character has
initiated or completed an actiion. Falling bombs, explosions, and the crab being hit
are trigger signals which felt cleaner than using global variables to pass information.

