# Class 3 Reading Notes

## Git Tutorial

Version Control is a system that allows you to revisit various versions of a file or set of files by recording changes.

The need for collaboration within a developer team on a single file or set of files led to the advent of the Centralized Version Control System (CVCS). 


A Distributed Version Control systems (DVCS) addresses the major vulnerability of the CVS: the server as a single point of failure.

Git mostly relies on local operations because most necessary information can be found in local resources.

Git traces its roots to the open source software project Linux kernel. Developers of this project began using a DVCS called BitKeeper in 2002. In 2005, many of these developers stopped using this DVCS due to tension between the Linux kernel community and the company behind BitKeeper’s and the eventual revocation of the DVCS’ gratis status.


Git includes inherent Graphical User Interface (GUI) tools. However, users can also utilize third-party tools created for particular platforms.

Without configuration of a default text editor, Git will use the system’s default editor–most likely Vim.

You can also create a copy of an existing Git repository from a particular server by using the clone command with a repository’s URL:

```
$ git clone https://github.com/test
```

Next, you would push changes to a remote repository. We will discuss remote repositories in more depth in the next section. For now, we will look at a general overview of pushing changes to remotes.


Almost every type of Version Control System incorporates branching. By creating branches of a central repository, collaborators are able to work on a project simultaneously via multiple branches, without affecting this main repository.

When you use the git merge --no-ff <branch> command, instead of a branch simply moving its pointer forward, a new commit object is created.


As we mentioned earlier, distributed workflows allow developers collaborating on projects much more flexibility. 

https://blog.udemy.com/git-tutorial-a-comprehensive-guide/