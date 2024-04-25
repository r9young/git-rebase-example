# Git Rebase Interactive Tutorial
This is an interactive tutorial on how to use the ```git rebase -i``` command to do the following:
- edit an old commit message
- delete an unwanted commit
- squash/combine multiple commits

## Warning about Git Rebase
```git rebase``` is a "destructive" command. While old commits can be found in the reflog, 
the actions in this tutorial will often give new your commits new id hashes and will rewrite
the history of your branch. It's often a good idea to make a backup branch when you are new 
to interactive rebase.

It is also advised to not manipulate your git history for anything that has already been 
distributed to others via a remote branch. It is best used locally to clean up work you are
intending to commit in a pull request.

## Getting Started
To get started, you will want to clone this repository to your local machine. 
If you need help on this step, consult the
[github documentation on cloning a repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository).

Once you have the repository cloned to your local machine, you will need to open a terminal and navigate to 
your working directory.

- **On Windows**, I recommend ```Terminal``` using ```Powershell```. This comes out of the box with Windows 10+.
- **On Mac**, I recommend [iTerm2](https://iterm2.com/) 
- **On Linux**, your life is terminal (and i don't mean ending, HAHA) so pick your own option.

## Edit An Old Commit Message

