---
title: Fun with Static Site Generators
published: true
layout: post
---

I recently listened to [a nice podcast][1] whose subject was Jekyll, the static site generator that powers this site. This got me thinking about how I got into Jekyll and why I've been using it. 

There seems to be a movement afoot to bring blogging back to basics. Although blogging engines with tons of features (like the ubiqitous [WordPress][2]) still power most of the online publishing going on many folks (especially the nerdier ones) are opting for simpler designs, fewer features and a focus on site performance and ease of reading over bells and whistles. The growth of static blog generators like [Jekyll][3] is part of this trend and [many other static site generators][4] have cropped up as well. The advantages of static site generators make up for the bit of extra effort it takes to compile them locally:

1. Page requests are super fast since they don't require generation of blog pages on the server. 
2. Static sites can be hosted on any web server with no extra dependencies. This site is hosted as a set of github pages, which gives me free hosting and CDN. 
3. The transparency afforded by a static site generator affords all kinds of opportunities for tinkering. [Brett Terpstra][5], the guest of the aforementioned podcast, has used Jekyll to produce a blog with tons of functionality and features (it takes over 10 minutes to build the thing). Static sites tend to share a certain aesthetic, characterized by simple lists of posts, sometimes even lacking an archive. This aesthetic has its apotheosis in the retro community created by [Tilde.Club][6], a collection of pages running as different home directories on a single Linux box. Many of those sites employ designs reminiscent of the text only interface of the Internet before the World Wide Web. 

There does seem to be a realization that more is not always better and that blogs are for reading, rather than commenting on, liking, pinging, etc. Most of all writers are finding that the old way are sometimes the best that the process of putting words together does not require powerful server architecture. I'm very happy with the Jekyll setup and would recommend it to anybody who want to get a site served as quickly and simply as possible.


[1]: https://mijingo.com/podcast/cms/jekyll
[2]: https://wordpress.com/
[3]: http://jekyllrb.com/
[4]: https://staticsitegenerators.net/
[5]: http://brettterpstra.com/
[6]: http://tilde.club/