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
## We're Going to Talk About Another Option...

(I use it a lot; maybe it'll be useful for you too)
	</section>
</section>

<section markdown="block">
	<section markdown="block">
## Um, What?

What's this all about now?

* [GitHub Pages](https://pages.github.com) (a feature on GitHub)
* allows you to host a site and manage its content...
* based on your project's repository
	</section>
	<section markdown="block">
## Show Me!

Let's try changing the pages that these slides are hosted on.

(change this text here!)

(live demos never work... or maybe they do?)
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
## Why?

* need a site that's attached to a project on github?
* minimal web interface to manage content?
* hate using web pages to manage content, but love the commandline!? (um... _those people exist?_)
</section>

<section markdown="block">
## Introductions

* me
	* teach programming at NYU 
	* teach programming tools at City-Tech
	* ITP Alum
* you
	* git / GitHub experience?
	* commandline?
	* gems?
	* markdown?
	* jekyll?
</section>

<section markdown="block">
	<section markdown="block">
## This Presentation

first part lecture + other part hands-on

	</section>
	<section markdown="block">
## More About This Presentation

Obvs - about [GitHub Pages](https://pages.github.com) (a feature on GitHub)

1. a few quick demos
2. discuss tools used
	* git
	* jekyll
	* markdown 
3. and... your turn!
	* create a site on GitHub Pages
	</section>
	<section markdown="block">
## (this is going to be a bit loose... and possibly only marginally _coherent_)

I can tailor this talk/presentation/workshop to whatever works for you!
	</section>
</section>

<section markdown="block">
## Technologies Used

* __git__: version control software
* __GitHub__: a site that hosts git repositories
* __GitHub Pages__: a feature on GitHub that allows _project site_ hosting
* __jekyll__: a static web site generator
* __markdown__: simple text formatting __mark-up__ (?), less complex than html
* __the commandline__: for _everything_
* __rvm, ruby gems, commandline, homebrew__: optional-ish _infrastructure_ / _dependencies_... 

</section>
<section markdown="block">
## Using GitHub Pages

There are a few different ways to create sites using GitHub Pages.  They all require a repository on GitHub.

* generate a site
* start from scratch
	* using the web interface
	* using the commandline
		* plain html
		* with layouts, markdown
</section>

<section markdown="block">
## And Now for Some Demos...

* in GitHub speak, these are _project sites_
* they'll end up at http://username.github.io/projectname
* they'll start off __suuuper simple__
* but we'll ramp up to some __complicated stuff__
* expect a bunch of commandline stuff
</section>

<section markdown="block">
## Demo: A Generated Site

1. create a repository
2. settings &rarr; automatic site generator 
3. content and settings
4. check urlhttp://username.github.io/projectname
5. edit

</section>

<section markdown="block">
## Demo: From Scratch with the Web Interface

1. create a repository
2. create a file to bootstrap a branch (perhaps README?)
3. create a branch called gh-pages
4. create an html file
5. create a markdown file
6. check urlhttp://username.github.io/projectname
</section>

<section markdown="block">
## So... Here's Where the Fun Begins!

(or... maybe where it gets a _little_ difficult)

</section>

<section markdown="block">
## Demo: From Scratch with the Commandline

1. create a repository
2. git clone https://username@github.com/username/repositoryname.git
3. git checkout -b gh-pages
4. create an __.html__ file
5. status, add, commit
6. git push -u origin gh-pages
</section>

<section markdown="block">
## Demo: From Scratch with the Commandline

1. \_layouts folder
2. {{ content }} tag
3. create a __.markdown__file
4. yaml front matter
5. markdown!
5. status, add, commit
6. git push -u origin gh-pages
</section>

<section markdown="block">
## Demo: Layouts

1. \_layouts folder
2. {{ content }} tag
3. create a __.markdown__file
4. yaml front matter
5. markdown!
5. status, add, commit
6. git push -u origin gh-pages
</section>

<section markdown="block">
## ...Now for Some Details on Concepts / Tech

* GitHub Pages
* git
* jekyll
</section>

<section markdown="block">
## GitHub Pages

* takes what's on your __gh-pages__ branch from your __git__ repository
* processes it through a static site generator, __jekyll__
* ...and hosts resulting files on github.io

Kind of makes sense?
</section>

<section markdown="block">
## git

* __git__ - the distributed version control system that we're using (why?)
* __GitHub__ - a website that can serve as a remote _repository_ for your project
* git != GitHub (__they're not the same thing!__)

</section>

<section markdown="block">
## git concepts

* __repository__ - the place where your version control system stores the snapshots that you _save_ (can be __local__ or __remote__)
* __branch__ - a _copy_ of your work that can be modified in parallel with other copies
* __stage__ - preparing your work to be saved
* __commit__ - saving your work
</section>

<section markdown="block">
## Some Commands

* __git clone__ - create a  _copy_ of a repository
* __git checkout -b branchname__ - create a branch
* __git status__ - what changed your repository?
* __git add__ - get ready to save your work (stage)
* __git commit__ - save
* __git push origin gh-pages__ - send your changes to a remote repository named origin
</section>

<section markdown="block">
## Side Note

Most people use git with __ssh keys__.  We'll use HTTP auth for now (hence the username@ before the repository urls)
</section>


<section markdown="block">
## jekyll

* it's a commandline program (a ruby gem!)
* than transforms/processes source files into ...
* dumps transformed into \_site
</section>

<section markdown="block">
## jekyll Continued

1. copies everything in your directory... 
2. into a folder called \_sites
3. it'll skip some things, directly copy some files... and transform others
</section>


<section markdown="block">
## Directory Layout

* \_layouts directory
* \_site directory
* \_config.yml
* prefix with underscore means it doesn't get dropped into the \_site folder
</section>

<section markdown="block">
## jekyll Commands

* jekyll build
* jekyll serve
* jekyll serve --watch
</section>


<section markdown="block">
## Files / YAML Front Matter
_yaml front matter_ tells jekyll that it should transform the page (not just copy directly

* must be at very beginning of file
* starts and ends with three dashes
* yaml between
	* __layout__: layout file to use
	* __title__: page title
</section>

<section markdown="block">
## Available Variables and Tags

* __content__ ... where your actual file is inserted into a template
* syntax highlighting
* includes
</section>

<section markdown="block">
## Let's Try This Together

1. Install some tools....
2. Create a site with GitHub PAges!

(This could be __disastrous__!)
</section>

<section markdown="block">
## Installing Git

Use [Homebrew!](http://brew.sh/)

(or a [graphical client](http://www.sourcetreeapp.com/))

(or ports... or whatever)

</section>

<section markdown="block">
## Installing jekyll

Use rvm!

* rvm list known
* rvm install ruby\_version
* rvm uninstall ruby\_version
* rvm use ruby\_version
* rvm \-\-default use ruby\_version
* rvm default (switch to default)
* rvm gemset list
* rvm gemset list\_all
</section>

<section markdown="block">
## Installing jekyll Continued

* https://pages.github.com/versions/
* gem install jekyll -v 1.5.1
* or install pages-gem
* gem install github-pages
</section>

<section markdown="block">
## Let's Make a Site!

...
</section>
