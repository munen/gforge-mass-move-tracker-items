Solved problem
--------------

There is no automated way of moving tracker items in [GForge](http://gforge.org). Each has to be moved by hand. This is a [iMacros](https://addons.mozilla.org/en-US/firefox/addon/3863/) script to automate this task, which has saved me a whole day of clicking repetitively.


Usefulness
----------

When you implement a new custom workflow in a legacy GForge environment, it is best to do so in a template. Every new project can then be cloned from it.

Unfortunately old projects will not get updated. You have two choices now: One is to repeat enforcing the workflow on every project (which is a tedious task and can easily take up to a day). The other is to make a new tracker which is cloned from the template. Then you can move your tracker items from the old tracker to the new one. Voila, you got the new workflow rules applied.


Usage
-----

 * Install iMacros in Firefox
 * Import this script into iMacros
 * Browse to the tracker in question (projects->tracker->[tracker name])
 * Open this iMacro script 
  * Configure the target tracker ID in !VAR1(note: this is a fixed iMacro variable name)
  * Configure your project unix name in !VAR2
   * You can see that in the URL: http://host/gf/project/[project name]/tracker/
 * Run the script
