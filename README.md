How to build the Aeolus Project website
=======================================

Requirements
------------

You need to have Ruby installed, along with the following gems:

* nanoc (3.3.3 is known to work)
* haml (3.1.4 is known to work)
* sass (3.1.16 is known to work)
* kramdown (0.13.5 is known to work)
* nokogiri (1.5.2 is known to work)
* adsf (1.1.1 is known to work)

Depending on your operating system, you may need to add the directory
with the "nanoc" executable to your $PATH.


Building the Website
--------------------

The Aeolus Project website is created using [nanoc][1]. It takes a website
defined by a set of layouts, templates and content files, runs a count
of filters on them and produces a static web structure that can be
directly posted to a webserver or displayed in a browser.

[1]: http://nanoc.stoneship.org

To do this, go to the "nanocsite" directory and run "nanoc compile":

    $ cd nanocsite
    $ nanoc compile

The website will be generated into the "nanocsite/output/" directory.

To view the output, start nanoc's built in web server, then point your
browser to http://localhost:3000.

    $ nanoc view
    $ firefox http://localhost:3000



Nanoc Help
----------

Nanoc has many more commands and options available.  You can find out more
about them by running:

    $ nanoc help



File Structure
--------------

* nanocsite/
 * the Aeolus Project website

* nanocsite/content/
 * the pages that are displayed on the website

* nanocsite/content/static-redmine
 * static redmine content (themes, javascripts, etc)

* nanocsite/layouts/
 * the Aeolus Project website template

* nanocsite/output/
 * the final version of the site -- this is what you want to view in a web browser



File Types
----------

* HAML files must have the extension .haml
* Kramdown files must have the extension .md

