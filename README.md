# Task2 Number Guessing Game

# Starting Branch Structure
Branch Structure: The number guessing game is structured with a main branch that maintains complete versions of the program, the dev branch maintains working versions of the program, the feature branches implement new features that can be added to the program, and the hotfix branch is used to implement hotfixes when necessary. 

    main branch: Initial Files 
    dev branch: Add a message to encourage players 
    feature1: Add the replay and quitting functionality 
    feature2: Add a limit to the number of guesses a player has before game over
    feature3: Add a hint mechanic to aid players with their guesses
    hotfix: Bugfix that enables the max value of the range of guessing numbers to be a possible solution 

* ab7cd7b (hotfix) Fix randomInt to properly include max value in range
| * 1f23d1c (feature3) done
| * 3631e47 had to fix
| * c070288 got it done
| * f1097b6 started hint
|/
| * e367776 (feature2) Implement max attempts logic and game over condition
| * 45aa640 Add maxAttempts constant and game over state
| * 5f95961 (dev) Add encouraging message for players
|/
| * f48cf81 (HEAD -> documentation, feature1) Add version comment documenting quit feature
| * 9df380f Improve user feedback messages for guesses
| * f8dfe81 Add play-again loop functionality
| * 3bbc201 Add ability to quit game with negative number input
|/
* 45767c4 (main) Initial Number guessing game



# Git Commands: Merge, Rebase, Squash, & Cherry-Pick (Uses)
Merge is used to integrate one branch into another branch while maintaining the commit history of both branches. If commits (changes) were made within the same logical chunks of a file in each respective branch a conflict occurs. Git will prompt the user to manually edit the file to determine whether to maintain the current branch's data, the merging branch's data, or both branches' data. Merge is used to integrate new features into a branch, ensure you are working with up to date files, and ensure your branch is in a working state before merging into the main branch. 

Rebase is used to create a linear commit history by superimposing a branch's commit history onto another banch's commit history. The commit history for the superimposed branch becomes altered as rebase rewrites the commits instead of preservering the initial commits. Rebase can be used as a tool to ensure you are working with up to date files while also maintaining a clean history. 

Squash is used to compress the commit log into fewer commits. Squash is great for when your commit log has become a mess and would benefit from a more accurate comment on what key change was made. Squash is also good for when you merge two branches to avoid creating an extensive merge log especially if most of the commits are not meaningful. 

Cherry-Pick is when you merge a specific commit from one branch into another. Cherry-picking is a great tool to use when you don't need to adjust several files and only need to update a small section of code in the current branch. This can be see with a hotfix that simply needs to be implemented within the main branch.

# Commit History: Feature1/Feature2/Feature3
Feature1's commit history was composed of the commits that occured on the feature1 branch as well as the dev branch commits after merging. An important note is the commit history of feature1 was maintained and a new commit was created to show the merging of dev into feature1. In the case of feature2 when it was rebased onto dev feature2's commit history was superimposed upon dev's commit history and the commits were rewritten instead of being saved as new commits. Lastly, with feature3 the commit history was condensed into a singular commit through the use of squash. Overall, feature1 maintained a more accurate commit history while feature 2 & 3 aimed for a cleaner and more linear commit history. 
