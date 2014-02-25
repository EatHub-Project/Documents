# SourceTree

SourceTree is a Git (and Mercurial) visual client. It helps with basic repository management for newcomers, and offers advanced features for experts. It also adds *git-flow* support out of the box and integration with GitHub services.

This is an optional tool for the development team. Each member can use the client they prefer, either visual or command-line based, but SourceTree is the recomended one. For command line git-flow support, visit [this website](http://danielkummer.github.io/git-flow-cheatsheet/).

For information about Git, visit the corresponding document under Technologies directory.

## Basic usage

### Important views

#### Sidebar

The sidebar provides a quick look into repository branches and remotes.
> Insert screenshot here

*Branches* lists local branches of the repository, organized in subfolders if any. It shows the current branch with **bold** format.

*Remotes* shows all the remotes of the repository, and it's branches. These branches are not meant to work on, only to fetch, pull and push commits.

*Stashes* shows saved stashes on the repository. They can be applied to the working tree from the list. Stashes are saved using the button in the toolbar.


#### File Status

This view shows the current status of the index and working tree. It's similar to the results of ```git status``` command. This is the principal view while working.

> Insert screenshot here

The left side is divided into *working tree* at the bottom, and *index* at the top. 

##### Working tree

The **working tree** lists edited, added and removed files, the ones that are not tracked yet. Selected files can be added to the index by pressing the *add* button in the toolbar. 

##### Index
The **index** shows the files (or changes) that are currently added to the repository index to be commited.

##### Diff
The right side shows changes in the selected file or files, similar to what ```git diff``` does. It displays added and removed lines within files, with a bit of context around them. 

> Insert screenshot here

This view allows to *stage* (add to the index) or discard changes line by line or hunk by hunk. This lets experienced developers futher customize what goes into a commit by staging some parts of a file, and leaving the rest for a different commit.

> *Hunks* are groups of nearby changes.

#### Log

The log view is divided in two main areas. The list of commits at the top, and information about the selected commit at the bottom.

The **list of commits** displays by default all the commits in all the branches, their author and the date they were made. It shows a multi-color graph to represent the conexion between commits and branches. It puts a litte tag before the commit to indicate the *current status* of a branch, its latest commit. From here the user can checkout or merge a specific commit.

Below the list SourceTree shows information related to the selected commit, such as the full commit message, changed files, and changed lines in the selected file.

### Common actions

### Examples