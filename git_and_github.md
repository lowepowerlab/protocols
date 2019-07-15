Content was forked and from [Mark Mandel/mjmlab](https://github.com/mjmlab/protocols/blob/master/git-github.md). A lot of content was removed to streamline, but it's not a bad idea to review it when we become more Git-competent. 

# Cloning and contributing to a lab Git repo on GitHub: `lowepowerlab/protocols` as an example

This is a bit meta: a protocol to demonstrate how to contribute to the protocols. It also serves as a model for working with other lab repositories.

<!-- TOC depthFrom:2 depthTo:6 withLinks:1 updateOnSave:1 orderedList:0 -->

- [What is a repository/repo?](#what-is-a-repositoryrepo)
- [Git vs Github](#git-vs-github)
- [Git and GitHub Setup and Basic Commands](#git-and-github-setup-and-basic-commands)
	- [GitHub signup](#github-signup)
	- [Play with GitHub](#play-with-github)
	- [Set Up a Text Editor on your computer](#set-up-a-text-editor-on-your-computer)
	- [Install Git on your computer](#install-git-on-your-computer)
	- [Modify a lab protocol](#modify-a-lab-protocol)

<!-- /TOC -->

## What is a repository/repo?

A repository (repo) in a directory or folder in which `Git` is tracking changes. It is an effective method for version control and to collaborate on code and documents.

## Git vs Github

Git is the language that facilitates the change tracking and merging. GitHub is a git server and associated website that facilitates collaboration and posting online.

## Git and GitHub Setup and Basic Commands

You can use Git on your own computer without the need for GitHub. However, since GitHub is a pretty and easy-to-use interface we will start there and then move to the command line Git interface on our computer.

### GitHub signup

1. [Sign up](https://github.com/join) for a GitHub account. 
1. [Sign up](https://education.github.com/discount_requests/new) for the GitHub educational discount. 
   - This will allow you to have private repos at no cost. 
1. Email Tiffany with your GitHub username so you can be invited to the [lab GitHub group](https://github.com/lowepowerlab). 

### Play with GitHub

See additional resources below to complete the following steps:

1. Look at the [Markdown language](https://daringfireball.net/projects/markdown/syntax), including the syntax particular for GitHub, aptly called [GitHub-flavored Markdown](https://guides.github.com/features/mastering-markdown/). The syntax is fairly simple, and this is widely used in GitHub documents, including our protocols.
1. Create a repo in your account via the web interface.
1. Make a change to the repo. This is called a "commit".
1. View the commit history of your repo.

### Set Up a Text Editor on your computer

Recommendation is `Visual Studio Code`
1. [Download `VS Code`](https://code.visualstudio.com/).
1. Install VS Code (or move to `Applications` folder on Mac).
1. Install Visual Studio code extensions like `Code Spell Checker`, `Excel Viewer`, `GitHub Pull Requests`, `Markdown Table Formatter`, `Python` (helps check your code), etc. 

### Install Git on your computer

1. On Mac, type `git config` on the command line (e.g., `Terminal` app) and if it is not installed you will be prompted to install the `XCode command line tools`, which includes `Git`.
1. [Here is information for other platforms](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) and more detailed information for Mac.

### Modify a lab protocol

Option 1: Follow the instructions on [Mark Mandel's Tutorial](https://github.com/mjmlab/protocols/blob/master/git-github.md#forking-and-cloning-the-protocols-repo).  

Option 2: If you want to frequently write & edit protocols, you can `clone` the protocols repository into VS Code & `push` changes to the `master` from your computer/account. 

* Open VS Code
* Ctrl+Shift+P to open the `search commands` dialog. Type "*clone*", hit enter.
* `Clone` the lab protocols github https://github.com/lowepowerlab/protocols. This will let you choose a local folder on your computer to view the lab protocols from. 
* Open the protocols `repo` in VS Code. 
* Edit a Markdown or other file (.md are markdown files)
* Save the Changes locally
* To commit to your git account, Open `Source Control` Menu (left). Add an informative description of the changes to the "Message", such as "*Fixed typos*", "*Improved clarity*", "*wrote protocol XXX*". Then `commit` by clicking the checkmark. Verify your changes have registered on the [`master`](https://.github.com/lowepowerlab/protocols)