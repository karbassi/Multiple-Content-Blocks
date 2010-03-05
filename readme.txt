Description
===========

With this plug-in, you can use more than one content "block" on a template. You only have to insert one tag inside the template, so its easy to use.

I made this plug-in because I think it is essential to any CMS to be able to use more content blocks in one template. I really missed this functionality in Wordpress and I did not find a decent plug-in for this, so I made one myself.

What is a "multiple content block"?
-----------------------------------

When you make a Wordpress template, you can show the content of the current page by using the code `the_content();`, but when you have (for example) several columns, you cannot split these in different content "blocks".

You want your clients to edit the content themselves without screwing up any code. This is where our plug-in comes in.

If you have any questions or tips, please contact me at harold@trendwerk.nl or leave  a comment on <a href="http://plugins.trendwerk.nl/">the blog</a>.


Installation
============

1. Extract the contents to the `/wp-content/plugins/multiple-content/` directory
2. Activate the plugin through the 'Plugins' menu in WordPress
3. Place `<?php the_block('blockname'); ?>` in your template where you want a content block
4. Edit this content on the page editing page

Frequently Asked Questions
==========================

How do I filter the content?
----------------------------

Use the function `get_the_block` instead of `the_block`, like this: `<?php $content_to_edit = get_the_block('blockname'); ?>` and you can now edit this variable with PHP.

Changelog
=========

1.4.1
-----
* Fixed a small bug when using MCB in Posts

1.4
---
* Now supports child themes!
* Fixed small php bug

1.3.1
-----
* Small bug fix when using `get_the_block`
* Fixed for WP 2.9

1.3
---
* Replaced `the_block('blockname',false)` by `get_the_block('blockname')`

1.2
---
Alot of bug fixes and small things

* You can now use multiple sidebars
* Added `the_content` filters
* Fixed the bugs with the default theme
* Posts are supported as well
* Double quote bug fixed
* HTML is better supported

1.1
---
* You can now use `the_block` in your (custom) header, footer and sidebar template files.

1.0
---
* Plugin created

Quick list
==========

* Create your own content blocks in a template
* Fill them with a WYSIWYG Editor