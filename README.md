# Git Rebase Interactive Tutorial
This is an interactive tutorial on how to use the ```git rebase -i``` command to do the following:
- delete an unwanted commit
- squash/combine multiple commits
- edit an old commit message

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
- **On Mac**, I recommend [iTerm2](https://iterm2.com/). 
I have a tutorial on [setting up a better terminal on macOS](https://davidboothe.com/a-better-terminal-on-mac-os/)
- **On Linux**, your life is terminal (and i don't mean ending, HAHA) so pick your own option.

## Delete an Unwanted Commit
Say you have a commit deeper in your commit history that you really don't want to push up
to everyone else working on your code base. You can use ```git rebase -i``` to alter 
the commit history and remove the unwanted commit before creating a PR.

### Identify the commit that we want to remove
Use the following command and look for the comment about adding azure credentials
```bash
git log -v
```
[insert picture here]

Now grab the hash of the commit AFTER the one we want to remove. 
You shouldn't need the whole thing, but the hash you are looking for should be
`3248590cd963d04618f734383c6d98db2a177132`

### Rebase Interactively
Add this hash to our rebase command

```bash
git rebase -i 3248590cd963d04618f734383c6d98db2a177132
```



## Squash / Combine Multiple Commits

## Edit An Old Commit Message

