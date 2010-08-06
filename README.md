What is this for?
================

With this appliance you should be able to start your symfony project in a minute. Nothing to installed and as this is a VM, all stuff is hold back from your normal system.

Features
========

 * phing - project automation and CI build tool
 * eAccelerator - php cache
 * subversion client - to pull symfony in
 * git-core - have a powerfull "no server needed" SCM tool
 * phpcs - code sniffer tool for static code analysis
 * phpunit - THE php test tool (standard in symfony2)
 * phpdoc - documentation generation tool
 * xdebug - debubbing extension for php

And additional to this a template project directory wiche enable kick ass fast project creation :D
See http://github.com/hoschi/tkl-symfony/tree/master/overlay/home/symfony/ for more details on this.

How to install
==============

Download the LAMP appliance from http://www.turnkeylinux.org/ and get TKLPatch from http://www.turnkeylinux.org/docs/tklpatch
After that you can path the LAMP iso by:
tklpatch tkl-lamp-hardy.iso tkl-symfony

Now you can install the iso in VM like VirtualBox or so.
