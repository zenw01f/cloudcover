.. _Git:
.. Title::
   Git

.. image:: images/git-icon.png
   :height: 100px
   :width: 100 px
   :scale: 50 %
   :alt: alternate text
   :align: left

Git
===
|
I don't have a lot on tutorials for Git but the Hello World page for Git will quickly have you become familiar with Git's basic structure.

.. toctree::
   :maxdepth: 2
   :hidden:

Tutorials
---------

* `readwrite's <https://readwrite.com/2013/09/30/understanding-github-a-journey-for-beginners-part-1/>`_ Git for beginners along with some basic CLI commands.
* `Git Immersion <http://gitimmersion.com/index.html>`_ course that is a good step by step you can follow along with.
* Youtube Videos on `Git & GitHub <https://www.youtube.com/playlist?list=PL4cUxeGkcC9goXbgTDQ0n_4TBzOO0ocPR>`_
* Introduction to the `GitHub Flow <https://guides.github.com/introduction/flow/>`_

Official Git Tutorials
^^^^^^^^^^^^^^^^^^^^^^
* `This <https://githubtraining.github.io/training-manual/#/01_getting_ready_for_class>`_ is the official GitHub Developer training manual.If you take the class from Git you'll be using this.
* `Hello World! <https://guides.github.com/activities/hello-world/>`_  - Git 10min activity. Good for getting your repo started.

Tips, Tools and CheatSheets
---------------------------

* `Tutorialspoint <https://www.tutorialspoint.com/git/index.htm>`_ learning site that is basically a decent reference page on Git commands
* The official `Git CheatSheet <https://services.github.com/on-demand/downloads/github-git-cheat-sheet.pdf>`_
* And a visual reference [ *just for BB8* ;-) ] of a `Git tutorial <https://marklodato.github.io/visual-git-guide/index-en.html>`_
* This presentation is a bit more historical and technical but if you're into that stuff `here ya go <https://raw.githubusercontent.com/pluralsight/git-internals-pdf/master/drafts/peepcode-git.pdf>`_
* `Git Everyday <https://mirrors.edge.kernel.org/pub/software/scm/git/docs/giteveryday.html>`_ is a quick reference guide that outlines 4 different types of roles for those who are working with git repositories.

Aliases
^^^^^^^
These are some links to useful aliases to add to your git config
* `GitHub Flow Like a Pro - 13 Aliases <https://haacked.com/archive/2014/07/28/github-flow-aliases/>`_


Shortcuts
---------
Some extra stuff I learned that were not on the man or help pages:

git config
^^^^^^^^^^
Creating an alias::

      $git config --global alias.s "status"

git checkout
^^^^^^^^^^^^
Create a new branch and checkout at the same time::

      $git checkout -b [new branch name]

git log
^^^^^^^
shorten git log output to just one one line::

      $git log --oneline

Add in a shorten status to the line with insertions/deletions/etc

      $git log --oneline --shortstat


Notes on Concepts
-----------------

I added this section for some more of the complex features of git.

Hunks
*****

Hunks are more like "chunks" of changes that you can do when you issue::

      git add -p

You will be prompted for each changed that you want added regardless of files.
It is a good way to review your changes or the individual changes per commit especially if you are sharing a file with other collaborators.

References for the -p (Patch) option and hunks: The Git Tutorial section on `Visualizing Changes <https://githubtraining.github.io/training-manual/#/17_view_local_changes>`_ helps to describe this.
