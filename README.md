Ping Pong Game Documentation:
This is the documentation for the Ping Pong game implemented in the provided HTML and JavaScript code.



HTML Structure:
The HTML structure of the game consists of a div container with an id of "game" that holds all the game elements. Inside the game container, the following elements are present:

Two paddles: paddle1 and paddle2. They are represented by div elements with the class "paddle" and unique IDs "paddle1" and "paddle2" respectively.

The ball: Represented by a div element with the ID "ball".

Score display: Two div elements with the IDs "score1" and "score2" are used to display the scores for player 1 and player 2 respectively.



CSS Styling:
The game elements are styled using CSS rules defined in the style section of the HTML code. The styles include:

The background color of the game is set to a dark blue color.
The game container has a width of 600px, a height of 400px, a border radius of 20px, and a white border.
The paddles are positioned absolutely within the game container and have a width of 10px, a height of 80px, and a background color of white.
The ball is positioned absolutely within the game container and has a width and height of 10px, a border radius of 50%, and a background color of white.
The score display elements are positioned absolutely within the game container, have a font size of 32px, use the Arial font, and have a white color.



JavaScript Logic:
The JavaScript code handles the game logic and user input. Here's an overview of the key aspects of the code:

Game State: The initial state of the game is set up with variables representing the positions, speeds, and scores of the ball and paddles.

Game Loop: The gameLoop function is responsible for updating the game state and rendering the changes on the screen. It is executed continuously using the window.requestAnimationFrame method, which provides smooth animation.

Ball Movement: The ball's position is updated in the gameLoop function by modifying the ballX and ballY variables based on the ballSpeedX and ballSpeedY values. The ball's direction is changed when it collides with the walls or the paddles.

Scoring: When the ball goes beyond the left or right boundaries, it is reset to the center, the score for the respective player is incremented, and the updated score is displayed.

Paddle Movement: The movePaddles function updates the paddle positions based on the user input received through keyboard events. The paddles are moved up or down by modifying the paddle1Y and paddle2Y variables. The paddles are constrained within the game area to prevent them from going out of bounds.

User Input: Keyboard events are used to detect when the user presses or releases certain keys (w, s, ArrowUp, ArrowDown) to move the paddles. The keydown and keyup event listeners are used to track the key states and update the paddle movement accordingly.

Game Initialization: The game loop and paddle movement interval are started using the window.requestAnimationFrame method and window.setInterval respectively.

How to Play
To play the game, follow these instructions:

Open the provided HTML file in a web browser.

The game will start automatically
