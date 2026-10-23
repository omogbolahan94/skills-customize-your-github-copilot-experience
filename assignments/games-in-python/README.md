
# 📘 Assignment: Hangman Game

## 🎯 Objective

Build a Hangman game that gives the player a limited number of chances to guess a hidden word. Practice using strings, loops, conditionals, user input, and random selection.

## 📝 Tasks

### 🛠️ Set Up the Hidden Word

#### Description
Create the word list and initialize the game so a randomly selected word is hidden from the player.

#### Requirements
Completed program should:

- Store at least five words in a predefined list.
- Randomly select one word from the list.
- Display one underscore for each letter in the selected word without revealing the word.
- Set and display a fixed number of incorrect guesses the player is allowed.


### 🛠️ Implement the Guessing Game

#### Description
Use a loop to let the player guess letters, update the displayed word, and finish the game when the player wins or runs out of guesses.

#### Requirements
Completed program should:

- Prompt the player to enter one letter on each turn.
- Reveal every occurrence of a correctly guessed letter in the word.
- Reduce the remaining guesses when the player guesses an incorrect letter.
- Display the current word progress and remaining guesses after each turn.
- End when the player reveals the whole word or has no guesses remaining.
- Display a win message when the word is guessed and a loss message that reveals the word when guesses run out.
