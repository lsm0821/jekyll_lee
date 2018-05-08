---
layout: post
title:  "Jekyll Cheatsheet"
date:   2018-04-30 00:32:32 -0700
categories: jekyll update
---
Jekyll Cheatsheet - by Sungmin Lee

![congrat](https://raw.githubusercontent.com/lsm0821/jekyll_lee/master/image/Project/New%20folder/jekyll.png)

Jekyll - A simple, blog-aware, static site generator.

![congrat](https://raw.githubusercontent.com/lsm0821/jekyll_lee/master/image/Project/New%20folder/rubygems.jpg)

Requirements:
1. [Ruby](https://www.ruby-lang.org/en/downloads/) version 2.2.5 or above.
  (You can check by running "ruby -v" at your terminal)
  After your download, you will see terminal that has a name of "Start Command Prompt with Ruby"
  This one is the terminal that I use to run a server for making my blog.

2. [RubyGems](https://rubygems.org/pages/download) (You can check if it is installed by running "gem -v" at your terminal)
Download a zip folder.
If you have a previous version of RubyGems, you can upgrade it by typing "gem update --system"

3. [GCC](https://gcc.gnu.org/install/) and [Make](https://www.gnu.org/software/make/) (you can check if you have them or not by running ("gcc -v"), (g++ -v), and (make -v))
(There is a high chance both GCC and Make are installed)

Starting Your Own Blog:

"gem install jekyll bundler" -- will install Jekyll and Bundler gems through RubyGems.
"jekyll new myblog" -- will create a new Jekyll site at ./myblog

(myblog is a name of your blog. If you can't find your file,
search it on window. it is usually in in driveC/users/yourname)

"cd myblog" - will change a current directory. (Basically means that you will move to this folder)

"bundle exec jekyll serve" - will build the site on the preview server

By completing steps up to here, Congratulation. Your blog is now ready.

<img src ="/site/image/Project/Alexa/Capture.PNG" alt="" class= "center">

After your Starting Point..

Typing "jekyll serve" at your command prompt will let your blog to run at its server.

Other useful commands are..

"jekyll serve --livereload" - this refreshes your browser after a change

"jekyll serve --incrementl" - this will perform a partial build in order to reduce regeneration time.

"jekyll serve --detach" - it will detach from the current terminal

If you want to kill the server - do 'kill -9 1234'/ '1234' is a PID.

However, if you can't find a PID, type "ps aux | grep jekyll"

Jekyll uses YAML for its Front Matter.
YAML: Tells Jekyll that it needs to process this file.

Examples:
"-,-,-"
layout: post
title: Blog
"-,-,-"

(But when you actually write it, don't include ','. I used it to separate three dash lines from forming a line.)

Some Available Variables:

date - A format of  YYYY-MM-DD HH:MM:SS +/-TTTT
example: date:   2018-04-30 00:32:32 -0700

category - specifying where post belongs to

You can use other textile format other than markdown.
Ex: HTML
