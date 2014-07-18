---
layout: default
title: Matt's Barkspy Build Notes
overview: true
---

# Matt's Barkspy Build Notes

You may download the changes via git using the command `git clone http://barkspy.mattrude.com/barkspy.git`

This repository currently has a branch for each different stage, below are the respective branches.

## original.barkspy.mattrude.com

The site [http://original.barkspy.mattrude.com/](http://original.barkspy.mattrude.com/) is as I downloaded the page on 7/7/2014.

No changes have been made to this branch (named 'master' in the git repo).

## css.barkspy.mattrude.com

The site [http://css.barkspy.mattrude.com/](http://css.barkspy.mattrude.com/) is my first update to the page.

This update is focused on css updates. With this update the site should be <a href="http://en.wikipedia.org/wiki/Responsive_web_design">responsive</a>.

* **7dd49f0** - Added favicon.ico <img src="https://raw.githubusercontent.com/mattrude/barkspy/master/favicon.ico?token=88956__eyJzY29wZSI6IlJhd0Jsb2I6bWF0dHJ1ZGUvYmFya3NweS9tYXN0ZXIvZmF2aWNvbi5pY28iLCJleHBpcmVzIjoxNDA1ODI5ODkyfQ%3D%3D--4db0ca58145e1c27edd4c724077f36622f643db4" alt="favicon.ico" title="" />
* **e951f17** - Updated base.css to a [LESS](http://lesscss.org/) file - [patch](./e951f17.patch)

## jekyll.barkspy.mattrude.com

The site [http://jekyll.barkspy.mattrude.com](http://jekyll.barkspy.mattrude.com) is a major change in the way the page is built. the source in this branch no long is a working website, but instead a true source directory.  You must use [Jekyll](http://jekyllrb.com) to build the site, but after the site is built, the server only servers static sites.

----
Updated: {{ site.time | date: "%m-%d-%Y" }} by [Matt Rude](http://mattrude.com).
