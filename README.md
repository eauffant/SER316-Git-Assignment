# Number Guessing Game

This project is a Java number-guessing game used to practice
Git branching, merging, rebasing, and conflict resolution.

## Initial Branch Structure

The project contains several branches, each representing
different stages of development.

### main
Contains the original version of the number-guessing game.
This branch represents the stable production version.

### dev
The development branch where features are integrated.
Initially includes an encouraging message for players.

### feature1
Adds the ability to quit the game using negative input,
play multiple rounds, and receive improved feedback.

### feature2
Introduces a maximum number of guessing attempts and
a game-over condition when the limit is reached.

### feature3
Introduces a hint system that helps players determine
how close their guesses are to the correct number.

### hotfix
Fixes random number generation to ensure the maximum
possible value is included in the range.

### documentation
Contains documentation describing the project,
branch structure, and Git workflows.

## Git Workflow Learning Summary



### Merge



Merging is used to combine changes from two different branches.

It keeps the commit history from both branches.



For this assignment, I merged dev into feature1 and had to fix

some conflicts in the Java code. After fixing them, I merged

feature1 back into dev.



I would use merging when working with other people on a project

because it keeps track of the changes made on each branch.



### Rebase



Rebasing is another way to combine changes from branches, but

instead of creating a merge commit, it moves the commits from

one branch on top of another.



I used rebase on feature2 to update it with the changes from dev.

I had to fix a few conflicts before the rebase could finish.



I would use rebasing when working on my own branch and wanting

to update it without adding extra merge commits.



### Squash



Squashing takes multiple commits and combines them into one.



For feature3, I had four commits that were all related to adding

the hint system. I squashed them into one commit to make the

history look cleaner.



I would use squashing when I have a lot of small commits that

are all part of the same feature.



### Cherry-Pick



Cherry-picking lets you take one specific commit from a branch

and apply it to another branch without merging everything.



In this assignment, I used cherry-pick to move a bug fix from

the hotfix branch into main. After that, I merged main into dev

so both branches had the fix.



I would use cherry-pick when I need to move a specific fix

without bringing over other changes.



## Differences Between the Feature Branches



### Feature1



For feature1, I used merging to bring in the changes from dev.

This created a merge commit that showed where the two branches

were combined.



After everything was working, I merged feature1 back into dev

and deleted the feature1 branch.



### Feature2



For feature2, I used rebase instead of merge at first.

This changed the commit history because Git created new commits

on top of dev.



I noticed that the history looked more straightforward compared

to feature1 since there wasn't an extra merge commit from

updating the branch.



Later, I merged dev into feature2 again to get the hint system

working with the maximum attempts feature.



### Feature3



Feature3 was different because I first combined four commits

into one using squash.



After that, I rebased feature3 onto dev and fixed the conflicts.



I noticed that feature3 had a much cleaner history because

the four original commits were replaced with one commit that

described the entire hint feature.



## What I Learned



This assignment helped me understand how Git handles changes

when multiple branches are being worked on.



The biggest thing I learned was how to resolve merge conflicts.

Sometimes both branches had code that I needed to keep, so I

had to figure out how to combine them without breaking the

program.



I also learned that merge, rebase, squash, and cherry-pick all

have different purposes. Which one I would use depends on

whether I want to keep the branch history, clean up commits,

or just move a specific change.



Running the Gradle tests after fixing conflicts was also

helpful because it let me check that the changes were

working before continuing.

