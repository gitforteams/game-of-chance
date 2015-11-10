# Git: A Game of Chance

A simple dice game to mimic commit manipulation in Git.

## Supplies

- One six-sided dice (or equivalent random number generator).
- One package of colour-coded dots -- with enough colours for each player to have a unique token. Buttons or beads would also work.
- One package of stars.
- One sheet of paper (A4 or A5 is fine) per player.
- One additional sheet of paper for the whole team.
- Approximately 4-6 humans.

## Playing the Game

- Distribute the sheets of paper and colour-coded dots to each player (represents the personal repositories).
- Put the remaining sheet of paper in the middle of the table (represents the central repository).
- Each player starts with four markers on their personal sheet of paper (and no markers in the central repository).
- In turn, each player rolls the dice and completes the required action.
- The game ends after the last person has successfully pushed their local repository to the remote (central repository in the middle of the table).

Dice outcomes:

1. Represents a local commit. All players add three tokens to their sheet. This is the only group action. Mimcis the git commands `add` and `commit`.
2. Represents a local mistake. Player who rolled the dice removes one token from the tip of their branch. Mimics the git command `reset`.
3. Represents "ready to share". Replace the last three tokens with a single token. Mimics the Git command `rebase --interactive`.
4. Represents "sharing with a private branch". Another player gains duplicates of your tokens. If you have not previously shared tokens, add a star to represent a merge commit. Mimics the git command `merge`. The star token mimics a merge commit (also available with `--no-ff`).
5. Update your work. Make a copy of all remote tokens from the central repository in your central branch. Mimics the git command `rebase`.
6. Represents share your work with the central repository. You may only share your branch if you have all the tokens in the remote repository. If yes, add your tokens. You are now "out" of the game. Congrats! If you don't have all the tokens locally, roll the dice again. If you roll a "5", you must update your personal game sheet with all the dots and then you may add your dots to the central repository. If you do not roll a "5", you must forfeit your turn and try again later.
