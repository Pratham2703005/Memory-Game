**Memory Card Game**

**Overview**
This project is a simple memory card game built using HTML, CSS, and JavaScript. The goal of the game is to match pairs of cards by flipping them over to reveal their images. The game keeps track of the player's score and maintains a record of the best score in the local storage.

**Features**
- Interactive UI with a radial gradient background.
- Card flipping animation.
- Score tracking and best score storage.
- Shuffle functionality to randomize cards at the start and on restart.
- Victory detection when all cards are matched.

**How It Works**

1.HTML Structure:
- The HTML file sets up the basic structure, including a title, score display, a grid container for the cards, and a restart button.
- The favicon and CSS styles are linked in the head section.
- The body contains the main elements of the game: a title, the grid container for cards, the score displays, and a restart button.

2.CSS Styling:
- The background is a radial gradient that transitions between dark shades of purple and red.
- The .grid-container displays the cards in a grid layout.
- The .card class defines the styling and flipping animation for the cards.
- The .scores and .actions classes align the score and restart button centrally.

3.JavaScript Functionality:
- Variables and Initial Setup:
  - The script initializes variables for handling cards, score, and best score.
  - The best score is retrieved from the local storage or set to a default high value if not available.
- Fetching Card Data:
  - Card data is fetched from a local JSON file (cards.json).
  - The fetched data is duplicated to create pairs and shuffled before being displayed.
- Card Generation and Event Listeners:
  - Cards are dynamically created and added to the grid container.
  - Each card has a front and back side, and an event listener for the flip action.
- Card Flipping Logic:
  - The flipCard function handles the card flipping animation and checks for matches.
  - If two cards are flipped and match, they are disabled. If not, they are flipped back.
- Score Tracking:
  - The score is incremented each time a card is flipped.
  - The best score is updated if the current score is better and saved in local storage.
- Restart Functionality:
  - The restart function resets the board, reshuffles the cards, and resets the score.
