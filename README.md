# Git Rebase Tutorial
This is an interactive tutorial on how to use the ```git rebase``` command to do the following:
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


