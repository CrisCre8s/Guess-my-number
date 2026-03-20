# Guess My Number!

A simple browser-based number guessing game built with vanilla JavaScript, HTML, and CSS.

## About

The game generates a secret random number between **1 and 20**. The player has **20 attempts** to guess the correct number. After each guess, the game gives feedback on whether the guess was too high or too low.

## How to Play

1. Enter a number between 1 and 20 in the input field
2. Click the **Check!** button to submit your guess
3. Follow the hints:
   - 📈 **Too high!** — your guess is above the secret number
   - 📉 **Too low!** — your guess is below the secret number
   - 🎉 **Correct Number!** — you won!
   - 💥 **You lost the game!** — you ran out of attempts
4. Click **Again!** to start a new round with a fresh secret number

## Features

- 🎲 Random secret number generated on every new game
- 📊 Score tracker that decrements with each wrong guess (starts at 20)
- 🏆 Highscore that persists across rounds within the same session
- 🎨 Background color changes to green on a correct guess
- 🔄 Full game reset via the "Again!" button

## Project Structure

```
project/
├── index.html       # Game layout and structure
├── style.css        # Styling and animations
└── script.js        # Game logic
```

## Getting Started

No installation or dependencies required. Just open `index.html` in your browser:

```bash
# Clone the repository
git clone https://github.com/your-username/guess-my-number.git

# Navigate into the folder
cd guess-my-number

# Open in browser
open index.html
```

## Game Logic Overview

| Condition         | Result                          |
|-------------------|---------------------------------|
| Empty input       | ⛔ Warning message shown        |
| Correct guess     | 🎉 Win state, highscore updated |
| Wrong guess       | Score decremented by 1          |
| Score reaches 0   | 💥 Game over                   |
| Again clicked     | Full reset, new secret number   |

## Built With

- HTML5
- CSS3
- Vanilla JavaScript (ES6+)

## License

This project is open source and available under the [MIT License](LICENSE).
