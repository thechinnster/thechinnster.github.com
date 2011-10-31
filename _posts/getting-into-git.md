---
published: false
layout: post
title: Getting into Git
---

Over the past few weeks I've been overtaken by a strange new obsession. I can't stop thinking about Git, the version control system created by Linus Torvald and used for developing the Linux kernel as well as numerous open source and private software development projects and other other of digital work ([even books](https://github.com/progit/progit "progit" "Progit book project on github")).

## Harder is better

One thing I like about got is that it is contains, for me, just the right amount of complexity. The basic operations are fairly simple but there are numerous parameters that can be added, configurations to be customized and advanced methods to be used. I've been researching and using Git for a couple of weeks and feel like I've just scratched the surface. That's one of the reasons I'm attracted to the system: it affords opportunities to learn and gain mastery. 

But it's not just advanced operations that are more challenging. Even the simple act of committing a file is more complex in Git than is other VCS like subversion. In  Git committing is a two step process: first you stage changes, then commit them. (Actually committing can be made simpler by using "commit -a" to add and commit a the same time but that isn't the default behavior.) Yes, this creates an extra step and so is "harder" than other systems but the benefit is worth it.  Staging changes together encourages you to be thoughtful about what is going into each commit. That pays dividends when you have to use your commit history later or somebody else needs to review your work. 

The same is true of the way that committing and pushing are two different steps. In a centralized VCS a commit will be automatically shared with everybody when they update from the centralized repository. In Git the commit happens locally and only gets shared when the local repository is pushed to another clone. In between the local history can be changed (commits squashed together, messages changed, etc.) in the interest of making the repository's history better for public consumption. This means that the user can commit fast and share slow. Those two tasks get treated differently because they are different and require different thought processes. You could say that this is harder than just committing changes and making them public at the same time and you'd be right, but easier is not better in this case. 

