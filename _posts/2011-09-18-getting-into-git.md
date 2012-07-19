---
published: true
layout: post
title: Getting into Git
---

Over the past few weeks I've been overtaken by a strange new obsession. I'm talking about Git, the version control system created by Linus Torvald and used for developing the Linux kernel as well as numerous open source and private software development projects and other kinds of digital work ([even books](https://github.com/progit/progit "progit/progit - GitHub")).  I've read [a number](http://progit.org/ "Pro Git - Pro Git Book") [of books](http://www-cs-students.stanford.edu/~blynn/gitmagic/ "Git Magic - Preface") [on the subject](http://book.git-scm.com/ "Git Community Book"), got myself a [github account](https://github.com/thechinnster) and even started evangelizing for Git at my svn using workplace.  I've never paid attention to any VCS before.  How did this happen? 

##### Harder is better

One thing I like about got is that it is contains, for me, just the right amount of complexity. The basic operations are fairly simple but there are numerous parameters that can be added, configurations to be customized and advanced methods to be used. I've been researching and using Git for a couple of weeks and feel like I've just scratched the surface. That's one of the reasons I'm attracted to the system: it affords opportunities to learn and gain mastery. 

But it's not just advanced operations that are more challenging. Even the simple act of committing a file is more complex in Git than is other VCS like subversion. In  Git committing is a two step process: first you stage changes, then commit them. (Actually committing can be made simpler by using "commit -a" to add and commit a the same time but that isn't the default behavior.) Yes, this creates an extra step and so is "harder" than other systems but the benefit is worth it.  Staging changes together encourages you to be thoughtful about what is going into each commit. That pays dividends when you have to use your commit history later or somebody else needs to review your work. 

##### Sharing is Caring

The same is true of the way that committing and pushing are two different steps. In a centralized VCS a commit will be automatically shared with everybody when they update from the centralized repository. In Git the commit happens locally and only gets shared when the local repository is pushed to another clone. M the local history can be changed (commits squashed together, messages changed, etc.) in the interest of making the repository's history better for public consumption. This means that the user can commit fast and share slow. Those two tasks get treated differently because they are different and require different thought processes. You could say that this is harder than just committing changes and making them public at the same time and you'd be right, but easier is not better in this case.

##### Digging In

I still work with Subversion, I have to since that's what's used in my office (at least until I win everybody over to Git).  Recently I have been using Git with git-svn (thanks to [this article](http://andy.delcambre.com/2008/03/04/git-svn-workflow.html "Git SVN Workflow")) so it acts as a client for the central subversion repository.  At last version control doesn't feel like a chore any more.  Every day there's a little satisfaction in using a tool better than I did before.  There's a host of decent GUI Clients, including my favorite, [Gitx](http://gitx.frim.nl/ "GitX - Home") but I find I'm using the command line more and more.  I want to be a power user not just a drone punching "svn commit" and "svn update" into my terminal all day.  Git has freed me up to be as nerdy as I want to be.    


