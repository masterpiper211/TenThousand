# Ten Thousand - Themed Edition

A web-based implementation of the dice game "Ten Thousand" (also known as Farkle). This version features switchable visual themes (Retro Pixel and Modern UI), sound effects, AI opponent option, and high score tracking.

## Play Online

[Link to live game deployment - *You'll need to host this yourself and replace this link*]

## Features

* **Classic Ten Thousand Gameplay**: Roll dice, score points, and try to be the first to reach the target score.
* **Multiple Players**: Play solo against an AI or with up to 4 human players locally.
* **Switchable Themes**:
    * **Retro Theme**: Pixel art font and a darker, nostalgic color scheme.
    * **Modern Theme**: Clean sans-serif font with a bright, contemporary interface.
* **Sound Effects**: Audible feedback for rolling, scoring, banking, busting, and winning (can be muted).
* **AI Opponent**: A basic AI provides a challenge for single-player mode.
* **Scoring Variety**: Supports standard scoring for 1s, 5s, three-of-a-kind, four-of-a-kind, five-of-a-kind, six-of-a-kind, straights, three pairs, and two triplets.
* **Hot Dice**: Score with all six dice and roll them all again!
* **Getting on the Board**: Players must score a minimum of 500 points in a single round to start banking their score.
* **High Score Tracking**: Saves the top 5 high scores locally in the browser.
* **Responsive Design**: Adapts to different screen sizes, suitable for desktop and mobile play.
* **Interactive Modals**: "How to Play" and "Scoring Guide" available in-game.

## How to Play

### Objective
Be the first player to reach the target score (default is 10,000 points).

### Getting Started
* Players must score at least 500 points in a single round to "get on the board." Until this threshold is met in one round, their scores cannot be banked.

### Your Turn
1.  **Roll Dice**: Click "Roll Dice" to roll all available dice (initially 6).
2.  **Select Scoring Dice**: After rolling, you *must* select at least one scoring die or a valid scoring combination of dice.
    * See the "Scoring Guide" in the game for point values.
3.  **Score Selected**: Click "Score Selected" to add the points from your selected dice to your current round score. The dice you scored are set aside for this round.
4.  **Hot Dice**: If all 6 dice are scored (in one or more selections), you get "Hot Dice"! You can then roll all 6 dice again and continue your turn.
5.  **Choose Your Next Move**:
    * **Roll Again**: Roll the remaining (unscored) dice to try and accumulate more points in the current round.
    * **Bank Points**: Add your current round score to your total game score. Your turn then ends.
6.  **Busting**: If you roll the dice and none of the resulting dice can be scored (a "Farkle" or "Bust"), you lose all points accumulated *in that current round*, and your turn ends immediately.

## Scoring Summary

* **Single 1**: 100 points
* **Single 5**: 50 points
* **Three 1s**: 1000 points
* **Three 2s**: 200 points
* **Three 3s**: 300 points
* **Three 4s**: 400 points
* **Three 5s**: 500 points
* **Three 6s**: 600 points
* **Four of a kind**: 1000 points
* **Five of a kind**: 2000 points
* **Six of a kind**: 3000 points
* **Straight (1-2-3-4-5-6)**: 1500 points
* **Three Pairs**: 1500 points (e.g., 2-2, 4-4, 5-5)
* **Two Triplets**: 2500 points (e.g., 2-2-2, 4-4-4)

## Running Locally

1.  Clone this repository or download the `index.html` file (or the full HTML code provided).
2.  Open the `index.html` file in a modern web browser (Chrome, Firefox, Edge, Safari).
3.  No server or build process is required as it's a single HTML file with embedded CSS and JavaScript.

## Code Structure

The game is contained within a single HTML file:
* **HTML**: Defines the structure of the game setup screen, game board, dice area, buttons, and modals.
* **CSS**: Embedded within `<style>` tags.
    * Uses CSS variables for easy theming.
    * Includes styles for both "Retro" and "Modern" themes.
    * Basic animations for dice rolling.
* **JavaScript**: Embedded within `<script>` tags.
    * **Game Logic**: Manages player turns, dice rolling, scoring calculations, AI decisions, and game state.
    * **DOM Manipulation**: Updates the UI based on game events.
    * **Sound Effects**: Uses `Tone.js` for synthesized sounds.
    * **Theme Management**: Handles switching and saving the selected theme.
    * **High Score Management**: Uses `localStorage` to persist high scores.

## Technologies Used

* **HTML5**
* **CSS3**
    * CSS Variables
    * Flexbox & Grid
    * Keyframe Animations
* **JavaScript (ES6+)**
* **Tailwind CSS** (CDN link for utility classes, though most styling is custom or theme-based)
* **Tone.js** (CDN link for Web Audio API sound synthesis)
* **Google Fonts** (for "Press Start 2P" and "Inter" fonts)

## Future Enhancements (Ideas)

* More sophisticated AI opponent strategies.
* Online multiplayer capability.
* More theme options or customizable themes.
* Advanced sound design or options for different sound packs.
* Keyboard controls for accessibility.
* Option for variant scoring rules.
* Save/Load game progress.

## Contributing

Feel free to fork this repository and submit pull requests with improvements or bug fixes.

## MIT License

