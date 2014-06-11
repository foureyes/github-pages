---
layout: slides
title:  GitHub - The Best CMS Ever (!?) 
---

<section markdown="block">
# GitHub - The Best CMS Ever (!?) 

(Using git and GitHub Pages to host a site _quickly_ and for free)
</section>

<section markdown="block">
## GitHub - The Best CMS Ever (!?) 

(While we wait)

* [follow along here...](http://foureyes.github.io/github-pages/)
* perhaps make an account on [github](http://github.com)?
</section>

<section markdown="block">
	<section markdown="block">
## Let's Talk About Web Sites

* hosting 
* static vs dynamic
	</section>
	<section markdown="block">
## There Are a lot of Options Out There!

...for hosting and creating sites.  For example:

* [Squarespace](http://www.squarespace.com/)
* [WordPress](https://wordpress.com/)
* [Weebly](http://www.weebly.com/)
* or, you know, 90's style... hand code and ftp to _your server_
	</section>
	<section markdown="block">
## This Talk is Kind of About the Modern Equivalent of That Last One

(hand code and ftp to _your server_)

(but sooo much better)

(and a bit more complicated, of course)
	</section>
</section>

<section markdown="block">
	<section markdown="block">
## Um, What?

What's this all about now?

* [GitHub Pages](https://pages.github.com) (a feature on GitHub)
* allows you to host a site...
* based on your project's repository
	</section>
	<section markdown="block">
## BTW, What's a Repository?

* within the context of version control... 
* it's where all historical versions of your work is stored 
* we'll see more later (maybe?)
	</section>
</section>


<section markdown="block">
## Some Examples

(yup, they're all hosted on GitHub Pages)

* [javascript games](http://basicallydan.github.io/skifree.js/)
* [Twitter's Bootstrap project page](http://twitter.github.io/bootstrap/)
* even my [Intro to Programming Course!](http://foureyes.github.io/csci-ua.0002-spring2014/)
* and of course, [this presentation](http://foureyes.github.io/github-pages/)
</section>

<section markdown="block">
## Introductions

* me
	* teach programming at NYU 
	* teach programming tools at City-Tech
* you
	* git / GitHub experience?
	* commandline?
	* gems?
</section>

<section markdown="block">
	<section markdown="block">
## This Presentation

Obvs - about [GitHub Pages](https://pages.github.com) (a feature on GitHub)

1. a quick demo
2. discuss tools used
	* jekyll
	* git
	* markdown 
3. and... your turn!

	</section>
	<section markdown="block">
## (this is going to be a bit loose... and possibly only marginally _coherent_)
	</section>
</section>
<!--
* what techs exactly?
	* just git and github really
	* ...but jekyll
	* markdown
	* obvs - html, css, etc. (i won't cover that)
* you?
	* who's used git?
	* who's used github?
	* who knows markdown?
* what we'll do:
	* set expectations so you'll know how long to stick around
		* 1 - hands-on
			* 1 - hands on stuff - git and github
			* 2 - other hands on stuff - templating and markdown
		* 2 - conceptuatl stuff
			* 3 - go over git and github in detail
			* 4 - go over templating and markdown
	* part 1 - git and github pages
		* create a github account (with email verified)
		* create a repository
	* part 2 - templating
	* part 3 - git and github concepts
		* git
		* github
	* part 4 - jekyll and markdwon
	


## jekyll
* what's jekyll again
	* it's a commandline program
	* than transforms/processes source files into ...
	* dumps transformed into _site
* testing
	* https://pages.github.com/versions/
	* gem install jekyll -v 1.5.1
	* or install pages-gem
	* gem install github-pages

* using rvm
	* rvm list known
	* rvm install ruby_version
	* rvm uninstall ruby_version
	* rvm use ruby_version
	* rvm \-\-default use ruby_version
	* rvm default (switch to default)
	* rvm gemset list
	* rvm gemset list_all
* directory layout
	* prefix with underscore means it doesn't get published (not sure, don't ask)
	* _layouts directory
* yaml front matter
	* yaml
	* three bars
	* layout:
	* title:
	* if it has, jekyll will transform / process it
* templating
	* available variables
		* page.title, etc.
		* content
	* tags
		* syntax highlighting
		* comments
		* includes
* config
	* using variables in config
## git
* homebrew 
-->
