
# 📘 Assignment: Hangman Game Challenge

## 🎯 Objective

Build a Hangman game that uses strings, loops, conditionals, random selection, and user input. Players will guess letters to reveal a hidden word before they run out of incorrect guesses.

## 📝 Tasks

### 🛠️ Set Up the Game

#### Description
Choose a hidden word from the provided word list and initialize the variables needed to track the game.

#### Requirements
Completed program should:

- Randomly select one word from the predefined `words` list.
- Track the letters the player has guessed.
- Set and track a maximum number of incorrect guesses.


### 🛠️ Run a Hangman Game

#### Description
Prompt the player to guess letters, show the hidden word's progress, and end the game when the word is guessed or no incorrect guesses remain.

#### Requirements
Completed program should:

- Repeatedly accept a letter guess while the game is still in progress.
- Display correctly guessed letters in their positions and use underscores for letters that have not been guessed (for example, `_ _ _`).
- Decrease the number of incorrect guesses remaining when the guessed letter is not in the hidden word.
- End when the player guesses the word or runs out of incorrect guesses, and display the appropriate win or lose message.
