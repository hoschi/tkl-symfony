What is this for?
================

With this appliance you should be able to start your symfony project in a
minute. Nothing to install and as this is a VM, all stuff is hold back from
your normal system, for save development.

Software
========

 * phing - project automation and CI build tool
 * eAccelerator - php cache
 * subversion client - to pull symfony in
 * git-core - have a powerfull "no server needed" SCM tool
 * phpcs - code sniffer tool for static code analysis
 * phpunit - THE php test tool (standard in symfony2)
 * phpdoc - documentation generation tool
 * xdebug - debubbing extension for php

Additional
==========

 * ready to use system developer
 * aware of chosen webserver and database (read "how to install" for more info)
 * simple .screenrc to give a better overview of your windows
 * template project directory wiche enable kick ass fast project creation :D
 * this include a bootstrap build.xml for phing usage
 * see http://github.com/hoschi/tkl-symfony/tree/master/overlay/home/symfony/ for more details on this.

Prerequisites
=============

This patch should work with almost all systems, because it has very simple dependencies:

 * a webserver to server your symfony projects
 * a database to store your data

There is one dependencie to apache2 in the post-overlay script which you can
delete if you don't have apache2 installed. On the other hand, if you want a simple LAMP stack,
uncomment the according lines:
http://github.com/hoschi/tkl-symfony/blob/master/conf/post-overlay

The LAMP appliance is available from http://www.turnkeylinux.org/.
You can find more web stacks on http://wiki.turnkeylinux.org/TKLPatch/Patches.
How ever, I tested it with TKL LAMP (ubuntu karmic - php 5.2) and TKL beta-core
(ubuntu lucid - php 5.3). 

How to install
==============
If you chosen your base image you can install TKL Patch from http://www.turnkeylinux.org/docs/tklpatch.
There is also an short usage guide by JedMeister in the TKL forum, see the link at the bottom. So far so good,
stop your running webserver and patch the LAMP iso by

	tklpatch tkl-lamp-hardy.iso tkl-symfony

Now you can install the iso in VM like VirtualBox or so.

When this is done and you have a running system, you must activate the symfony user with:

	passwd symfony

Without this you can't login to your machine with the symfony user! The symfony
user is the system user, which you should use for development. He is in the
www-data group. All you make group write-/readable can be accessed from the web
server. This provides more security than make the log and cache dirs in a
symfony project world writable.

At least you should visit the issue tracker on github -> http://github.com/hoschi/tkl-symfony/issues
And feel welcome to ask questions or discuss about ideas on the TKL forum -> http://www.turnkeylinux.org/forum/support/20100719/what-do-you-miss-php-developer-current-symfony-appliance


[![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/hoschi/tkl-symfony/trend.png)](https://bitdeli.com/free "Bitdeli Badge")

