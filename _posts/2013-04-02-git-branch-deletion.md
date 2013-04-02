---
title: Git Branch Deletion
published: true
layout: post
---

One great thing about git is that branching and merging are cheap. For this reason I create a lot of branches and there's a whole bunch of them sitting around in my repo and on the remote I share with my team. Many of these branches are out of date and useless, cluttering up the repository and making it more difficult to see branches that are still active. I had been deleting these one at a time but figured there had to be a better way. A google search later it was [Stack Overflow](http://stackoverflow.com/ "Stack Overflow") to the rescue.

First I wanted to clean up the remote repository. I found [this SO page](http://stackoverflow.com/questions/10555136/delete-multiple-remote-branches-in-git "bash - Delete multiple remote branches in git - Stack Overflow") that provided the following one-liner:

    git branch -r | awk -F/ '/\/PREFIX/{print $2}' | xargs -I {} git push origin :{}

Just replace PREFIX with the appropriate string and the matching branches will be deleted from origin. In my case feature branch names begin with Jira issue numbers so deleting a bunch using this method was a snap.

Then I needed to remove outdated local branches as well. Another line (given in [another SO thread](http://stackoverflow.com/questions/3670355/can-you-delete-multiple-branches-in-one-command-with-git "Can you delete multiple branches in one command with Git? - Stack Overflow")) will take care of that:

    git for-each-ref --format="%(refname:short)" refs/heads/3.2\* | xargs git branch -D

Now my local and remote repositories are cleaned up in minutes and I can do this easily again when it gets messy. Sweet!


