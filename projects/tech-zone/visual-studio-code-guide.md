---
layout: default
---
# Visual Studio Code Guidelines

## Contributors

**Author:** [Daniel Feller](https://twitter.com/djfeller)

## Overview

Using GitHub Desktop and Visual Studio Code helps simplify the creation of Tech Zone content. A set of rules is added to Visual Studio Code to validate proper markdown settings. In order to use this, the local environment must be set up and configured. This guide provides the steps needed to configure.

## Visual Studio Code Setup

1. Download and install Visual Studio code: [Visual Studio Download](https://code.visualstudio.com/)
1. Once installed, launch Visual Studio Code to install the correct extension. This extension, when configured properly, will look for errors in the markdown language.

    ![Visual Studio Code Extensions](/media/visual-studio-code-guide_vsc-extensions.png)

1. Search for the extension "markdownlint". Install
1. In the local file system, navigate to `%AppData%\Code\User` (Windows) or `~/Library/Application Support/Code/User` (Mac OS).
1. Create a file called "settings.json"
1. Edit settings.json in Notepad. Paste in the following rules (including the brackets)

```text
{

"git.enableSmartCommit": true,

"git.confirmSync": false,

"git.autofetch": true,

"markdownlint.config": {

"MD003": { "style": "atx" },

"MD007": { "indent": 4 },

"MD009": { "br_spaces": 2 },

"MD013": false,

"MD024":false,

"MD026": { "punctuation": ".,;:!" },

"MD030": { "ul_single": 2,

"ol_single": 2,

"ul_multi": 2,

"ol_multi": 2 },

"MD033": true,

"MD040": false,

}
```

1.  Save and close "settings.json"
1.  Close Visual Studio Code

**Note:** You can also download extension [Markdown All in One](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one). This extension adds various features to VSC, including ability to use common keyboard shortcuts (Ctrl + B), table of contents, auto preview or simplified link creation.

## GitHub Desktop Setup

1. Download GitHub Desktop [GitHub Desktop Download](https://desktop.github.com)
1. When prompted, sign in to GitHub
1. Select the Tech Zone repository and select clone. This process will take some time as a full clone of the Tech Zone is being stored on your endpoint.

    ![GitHub Repository Clone](/media/visual-studio-code-guide_clone.png)

## GitHub Desktop Usage

Once the clone is complete, you get to the main GitHub Desktop screen.

1. Select the correct repository.
1. Select the correct branch for your changes.
1. Select "Open in Visual Studio Code"

    ![GitHub Desktop Branch Selection](/media/visual-studio-code-guide_desktop-repo-branch-edit.png)

1. In Visual Studio Code, navigate to the correct article in the left-side navigation tree.

    ![Visual Studio Code Navigation](/media/visual-studio-code-guide_vsc-navigation.png)

1. As you edit, you can see an in-app preview of the page by typing the following key combination: In Windows use `Ctrl+K`, then type `V`. In Mac OS, use `Command+V`. 
1. As you edit in markdown, errors are shown with a squiggly line.  There is a warning triangle icon in the lower left identifying how many markdown errors are detected. Selecting the triangle provides additional details on the errors.

    ![Visual Studio Code Markdown Errors](/media/visual-studio-code-guide_md-errors.png)

1. If you select the triangle in the Problems section, Visual Studio Code will fix many of the errors for you.

    ![Visual Studio Code Markdown Corrections](/media/visual-studio-code-guide_error-help.png)

1. If you have images to add, right-click the correct media folder and select "Reveal in Explorer". Simply copy your files into the folder, making sure they are named according to standards.

    ![Visual Studio Code Media](/media/visual-studio-code-guide_reveal-explorer.png)

1. Once done modifying the GitHub page, select File - Save within Visual Studio Code.
1. Close Visual Studio Code
1. GitHub Desktop is now visible. You can see the changes you made to the current branch. Add a brief description and select Commit.

    ![Visual Studio Code Commit Changes](/media/visual-studio-code-guide_commit-changes.png)

1. These changes are only stored locally. You need to push them to GitHub by selecting "Push Origin".

    ![Visual Studio Code Push Origin](/media/visual-studio-code-guide_push-origin.png)

You can continue modifying files within this branch according to your project. Once done and ready to publish, make sure the final updates are pushed to origin, then inform the Slack channel for publication.

Once the upload to GitHub is complete, verify the page renders properly by going to page within the browser.

## Summary

Below is summary overview of steps required to publish content on GitHub. Don't remember - until you **Push** your changes, central GitHub is not updated.

- **Commit** - Save changes to your local database
- **Push** - Upload changes from your local database to central database (GitHub)

    ![Visual Studio Code Process Overview](/media/visual-studio-code-guide_process.png)
