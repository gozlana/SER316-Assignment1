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

## Git Operations Performed

### Merge

I merged `dev` into `feature1` and resolved the conflicts. After testing the changes, I merged `feature1` back into `dev` and deleted the completed feature branch.

I also merged `dev` into `feature2` to combine the maximum-attempts functionality with the quit and hint systems. After resolving conflicts and passing the tests, I merged `feature2` back into `dev`.

### Rebase

I rebased `feature2` onto `dev` and resolved the conflicts. I also rebased `feature3` onto `dev` after squashing its commits.

Rebasing moves a branch's changes onto a new base and creates a more linear commit history.

### Squash

I combined the four development commits on `feature3` into one commit:

`Add hint system to show proximity after 3 attempts`

Squashing makes the history easier to read by combining related commits into a single commit.

### Cherry-pick

I cherry-picked the hotfix commit onto `main` to correct the random-number generation. I then merged `main` into `dev` so the development branch also received the fix.

Cherry-picking applies a specific commit without merging the entire branch.

## What I Learned

This assignment helped me understand how Git manages changes across multiple branches.

- **Merge** combines work from different branches while preserving their development history.
- **Rebase** reapplies commits onto another branch and can create a cleaner, linear history.
- **Squash** combines several related commits into one.
- **Cherry-pick** applies an individual commit to another branch.

I also practiced resolving merge conflicts, running Gradle tests, and verifying that different features work together.

In a real software development team, these Git operations help developers collaborate, integrate features, maintain readable commit histories, and apply important bug fixes.