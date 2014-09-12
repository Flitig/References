References
==========

My reference stuff. Happy to share, but really only writing them for my personal use.   :-)

GIT
===

This whole thing depends on an actual github-repo already created.


Get your repo to your local machine
-----------------------------------

Be sure to have your ssh-keys in order. Go to the repo on Github and copy the URL (you can find this in the right
column)

Then stand in the folder where you want your project to be located and type:

``$ git clone <copy from clipboard>``

Now you will have set up a master branch on your computer that is tracking the corresponding master branch on your
repo on github.

To update your machine with changes on Github, stand in the right folder in you terminal and type:

``$ git pull``

To update your repo on Github with changes you've made to the code on your machine, stand in the right folder in you
terminal and type:

``$ git push``



Create a new branch
-------------------

**Create a new branch that's tracking a new corresponding branch on origin**

Be sure to stand in the branch you want to branch out from and that it is up to date.

``$ git checkout -b <name>``
``$ git push -u origin <name>``


**Grab an existing branch from origin and create a local version that's tracking it**

``$ git checkout -b <name> origin/<name>``

Remove a branch
---------------

**Remove a branch from origin**

Be sure to stand in the branch you want to remove.

``$ git push origin :<name>``


**Remove a local branch**

``$ git branch -d <name>``

If you get a message complaining about where your HEAD is, you can force this by:

``$ git branch -D <name>``

Take what you need
------------------

**Grab a file from another branch into yours**

Be sure to stand in the branch you want to collect the file into.

``$ git checkout <name of other branch> <file name>``


**Update your branch**

This can cause merge conflicts.

Do a pull to develop to get the latest changes. Be sure to stand in the local branch you want to update.

``$ git merge develop``
