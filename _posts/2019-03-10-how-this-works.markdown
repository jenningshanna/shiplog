---
layout: post
title:  "How this works"
date:   2019-03-10
categories: fun poetry
lead: "A site is a site is a site"
---

Here are all the services that make this site work.

[Nearly Free Speech](https://nearlyfreespeech.com)<br />
First off, we use Nearly Free Speech. A hosting and name registration service that is operated by it's members. It's brilliance is in that it only charges you for the data you consume on their servers. It's also has an interface that hasn't changed in forever so once you're used to it like I am you probably don't want to even think of using anything else.

[Github](https://github.com/jenningshanna/shiplog)<br />
The second service we use it GitHub. The greatest thing to ever happen to code. If you don't know what GitHub does here's the gist. You put code there (like this site) and it keeps a record of it. This is really handy considering that code is full of dependencies of other services (for example the multiple services that stand up this site) to have this kind of redundancy. I'm using GitHub as a repository for all this code.


[Github Pages](https://pages.github.com/)<br />
Next is GitHub Pages. I know what you're thinking... "wait you just said GitHub". But GitHub Pages is a separate service that allows me to link this subdomain you're on (shiplog.jenningshanna.com) with a GitHub repository. How this works is that we create a DNS record over at Nearly Free Speech, and we create a CNAME matching that DNS in a our repository, then we tell GitHub Pages that those things exist and it checks them and publishes the site when we update the repositories master branch (master branch refers to the main development area of the repository).

[Hard Code Integration](http://blog.justsophie.com/automatic-website-deployment-with-git-hooks/)<br />Then we use this persons amazing code to tell Nearly Free Speech to update to reflect our latest public repositories state. In plain english, that means when we update GitHub we will update the site automatically. Like magic! Well actually we are telling the git remote to ping Nearly Free Speech SSH and ask us to login and publish while we update the master branch of our repository. Still magical!

[Jekyll](https://jekyllrb.com/)<br />Last and most importantly, we use Jekyll. Jekyll is a combination of Markdown, Liquid, YAML, HTML, SCSS, and a few other technologies wrapped in a nice site building package. It's important because we can deploy a server locally, create generative and dynamic content, and structure semantics easily. This allows for things like date, author, and topic categorization. This is hugely important as sites can have hundred of pages and we don't want to have to update them all manually every time we change a topic name of wether or not something is in the navigation.

And that's it. I hope someone finds this helpful for building your own site. If you do, please share it with [me](https://twitter.com/jenningshanna). Thanks!