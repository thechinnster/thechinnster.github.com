---
title: Post to Github Pages Jekyll Workflow
published: false
layout: post
---

This blog is running on [github pages][1] which uses the [jekyll templating engine][2] and thus nicely generates a blog style site every time I push commits to the pages repository. This gives me a lot of benefits, including free and robust hosting and the ability to write blog posts in [Markdown ][3] in plain text files that are easily editable and portable. The one downside is that there's a bit of overhead in having to commit and push all changes to get a post published. With so many publishing tools easily available on mobile devices, I've been looking for a way that I can easily post to this site from any device, anywhere. [In an earlier post][4] presented a possible way to publish remotely but it required using a few different apps and was fairly cumbersome; since my initial test I haven't used the workflow once, a state of affairs which doesnt speak well for it's usefulness. Since then I've found a much simpler method that only requires that I save any files to be published in a specified folder. 

This workflow requires [Dropbox][5] and [Hazel][6]. Initially I tried putting my whole blog directory in Dropbox but since the blog is in a git repository this got a little messy. Instead I'm using Hazel to move posts from a Drafts folder in Dropbox to the _posts folder for my jekyll blog. Rules are set up so that only files with correctly formatted names — beginning with a date stamp —  are moved. The filename match rules make it easy to detect files that start with a date without having to resort to regexes. After moving the file  Hazel runs a script to add and commit the new file and then push the repository to github. Running this on my iMac at home I can publish from my iPhone or iPad (using [Byword][7] or [Editorial][8]) or any other computer with access to my Dropbox. I use a file name with no date stamp while writing and then add today's date when I'm ready to publish. 

<figure><img src="https://files.app.net/9vspzpOJ.png" alt=""> <figcaption>The "jekyll" format is one I set up as the date stamp necessary for post file names</figcaption></figure>

I was trying out [scriptogr.am][9] but customizing it seemed like a pain and I'm not too confident about using a hosted service that doesn't charge me anything (and has no other apparent way of generating revenue). Now my jekyll blog gives me all the flexibility of a locally managed site that I can publish to at will with the push of a button (or the save of a file).


[1]: http://pages.github.com/
[2]: http://jekyllrb.com/
[3]: http://daringfireball.net/projects/markdown/
[4]: http://benchinn.com/2013/09/26/mobile-posting.html
[5]: https://www.dropbox.com/
[6]: http://www.noodlesoft.com/hazel.php
[7]: http://bywordapp.com/
[8]: http://omz-software.com/editorial/
[9]: http://scriptogr.am/
