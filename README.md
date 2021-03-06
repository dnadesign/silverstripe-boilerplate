# SilverStripe Framework Boilerplate

This project contains boilerplate code for various types of SilverStripe 
installation. It's structures so that each git branch contains a different 
boilerplate template to start from.

## Requirements

* PHP 5.3+
* Git
* Composer (http://getcomposer.org/)

## Installation

To start a new project on the boilerplate run the following from your terminal
(unix only) for the automatic install:
	
	bash <(curl -s https://raw.githubusercontent.com/dnadesign/silverstripe-boilerplate/master/install)
	
Or you can install manually by performing the steps below:

	git clone git@github.com:dnadesign/silverstripe-boilerplate.git my_app
	cd my_app
	./install

## Boilerplate templates

### master

Master branch includes boilerplate for a framework only application (no cms 
module). This branch describes basic controller and routing examples.

### cms

Includes boilerplate for a basic CMS powered website.

### foundation

Uses the ZURB [Foundation module](https://github.com/ryanwachtl/silverstripe-foundation) 
and the Foundation Forms module from Ryan Wachtl to provide a bootstrap of 
prototype design styles.

## Discussion

### app instead of 'mysite'

Shorter, cleaner, betterer than mysite.

### No themes folder.

Some branches (cms, framework) do not use a `themes` directory. We prefer not to 
use the `themes` directory as keeping templates all in app allows me to reduce 
the amount of root folders as well as keep projects tidier. 

Since most framework only apps won't be using different themes, it seems 
redundant to separate templates like that.

## Recommended Modules

Below are modules we use on most framework application projects and have been 
tested without the cms module.

* silverstripe/sqlite3 - for faster unit tests
* silverstripe/googlesitemaps - create a sitemap.xml file for your URLs

## Contributions

Contributions, extensions and other improvements are welcome via pull request. 
Please include which branches you would like to merge against (i.e master and 
cms) and we'll cherry pick between branches rather than raising multiple pull
requests.

Follow the coding conventions at http://doc.silverstripe.org/framework/en/trunk/misc/coding-conventions.
