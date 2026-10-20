# Number Guessing Game — Git Assignment

## Initial Branch Structure

This project uses Git branches to develop and manage different features of a Java number-guessing game.

- **main:** Contains the original number-guessing game.
- **dev:** Adds an encouraging message for players and serves as the integration branch.
- **feature1:** Adds the ability to quit using a negative number, a play-again loop, and improved feedback messages.
- **feature2:** Adds a maximum-attempts limit and game-over logic.
- **feature3:** Adds a hint system to help players guess the number. This branch initially contains four development commits.
- **hotfix:** Fixes the random-number generation so the maximum value can be included in the range.

## Branching Strategy

The main branch represents the stable version of the game. The dev branch integrates completed features. Feature branches allow changes to be developed separately before merging. The hotfix branch contains a correction that can be applied to main.