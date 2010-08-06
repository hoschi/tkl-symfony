how to use
================================================================================
The template project has a simple directory structure:

 * ./code  -> here goes all code stuff
 * ./build -> here goes all generated stuff during a build 

You only must copy the "template" dir to a new location and run the "init-firsttime" task.

	cd ~/
	cp -r template test
	cd test/code
	phing -l
	phing init-firsttime


This

 * installs symfony 1.4
 * sets up dirs normaly not checked in, in you code repository

You can also copy the files located in ~/template/code in you existing project to make use of this.

After you downloaded symfony you can use the other tasks in the build file. A "phing -l" lists all
available tasks. These tasks are include/exclude the std symfony files which you don't wanna in
your coverage analyses, api doc, and so on.

