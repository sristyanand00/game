Overview
This documentation outlines the structure, functionality, and logic of the Memory Game, a simple browser-based card matching game using HTML, CSS, and JavaScript. The goal of the game is to match pairs of emoji cards by flipping them.
HTML Structure
Elements:
1. Container (<div class="container">):
Holds the game title, game board, and reset button.
2. Game Board (<div class="game">):
Placeholder for the card grid dynamically populated by JavaScript.
3. Reset Button (<button class="reset">):
Refreshes the page to restart the game.
JavaScript Functionality
Key Components
1. Emoji Array
 An array containing pairs of emojis to serve as the cards in the game.

2. Shuffle Function
 Randomly rearranges the emoji array to ensure different card placements in every game.

3. Card Generation
    Creates a grid of <div> elements representing cards.
Each card is assigned a hidden emoji via the data-emoji attribute.

4. Card Click Handler
 Clicking a card reveals its emoji.
A boxOpen class is added to track flipped cards.

5. Matching Logic
Compares the inner HTML of the two flipped cards.
If they match, a boxMatch class is added to mark them as matched.
If all pairs are matched, the player wins.

6. Resetting Unmatched Cards
   If the flipped cards don't match, they are flipped back after a delay.
   
7. Game Reset Button
Reloads the browser window, resetting the game.

Additional Functions:

checkForMatch()
Checks if two selected cards match.

disableCards()
Disables interaction with matched cards.

unflipCards()
Resets the state of unmatched cards.

resetBoard()
Resets internal variables for card tracking.
