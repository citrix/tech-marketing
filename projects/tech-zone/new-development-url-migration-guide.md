---
layout: default
---
# New Tech Zone GitHub URL - Migration Guide

**Author:** [Phil Wiffen](https://twitter.com/phil_wiffen)

## Overview

This guide covers how to migrate your Tech Zone development from using the martinzugec-ctx organisation, to the citrixtechzone Github location, if you're using using GitHub Desktop and Visual Studio Code.

## Conceptual steps

You will need to change your git development environment so that it points to the new github location.

To do this you’ll need to:

1.  Clone the new repository in GitHub Desktop, which will get the new location on your local computer
1.  Remove the old repository from your local file system – so that you don’t accidentally develop in there once migrated.

## Clone the new repository in Github desktop

1.  Open GitHub Desktop
1.  Either press Ctrl+T to bring up your repositories, or click on the "Current repository" drop down in the UI
1.  Clone the new repository location by choosing Add > Clone Repository
   ![Clone Repository](/media/new-development-url-migration-guide_clone-repository.png)
1.  In the popup, choose URL and then paste in the following URL: <https://github.com/citrixtechzone/en-us-tech-zone>
1.  If you get a warning that "This folder contains files" - it's because GitHub Desktop is going to put the clone into the exact same folder you had the older repository cloned to.
    ![Files exists warning](/media/new-development-url-migration-guide_files-exist-warning.png)
1.  To fix this, click "Choose..." and choose a new location for the cloned repository. I chose to name the folder "citrixtechzone_en-us-tech-zone", so it looks like this:
    ![Rename local repo](/media/new-development-url-migration-guide_rename-local-repo.png)
1.  Click Clone to clone the new repository to your local machine
1.  If asked how you plan to use the fork, say "For my own purposes". This ensures that GitHub Desktop will submit changes (pull requests) into the citrixtechzone en-us-tech-zone repository, which is the correct place (because most contributors do not have access to contribute to the citrix en-us-tech-zone repository - and publishing to that location is controlled by automation from the Tech Zone team)
    ![Fork choice](/media/new-development-url-migration-guide_rename-fork-choice.png)
1.  Click Continue.

## Remove the old repository

Remove the old repository that is under martinzugec-ctx by:

1.  Click on the Current Repository drop down.
1.  Right click on the repository, and choose "Remove..."
   ![Remove repo](/media/new-development-url-migration-guide_remove-old-repository.png)
1.  Choose to move the repo to the Recycle bin if useful/available - this way you can get it back later.
    ![Remove repo popup](/media/new-development-url-migration-guide_remove-old-repository-popup.png)

## Developing from the new location

1.  You can now change the Current repository to the new one under citrixtechzone and develop articles from there, the next time you request a branch.

![switch to new repo](/media/new-development-url-migration-guide_switch-to-new-repository.png)
