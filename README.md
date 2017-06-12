Author Carpentry : Using Markdown and github to author for web and print
=======

*Content Contributors: Sebastian Karcher*

*Lesson Maintainers: Sebastian Karcher*

**Lesson status: In Development**

## Learning Objectives:
- Using Jekyll to transform markdown into webpages
- Creating a github page with simple navigation
-
<!--- Setting up a workflow to create both html and PDF/ebook version -->

## Topics:

1. [Topic 1: Getting Started](00-getting-started.html)
2. [Topic 2: Markdown Syntax](01-markdown-syntax.html)
3. [Topic 3: Github Pages](02-gh-pages.html)
4. [Topic 4: Jekyll Setup (optional)](03-jekyll-setup.html)
5. [Topic 5: Site Structure](04-site-structure.html)
6. [Topic 6: Changing your site theme](05-changing-theme.html)

<!--### Optional
- [Topic 5](04-services.html) -->


## Requirements

Author Carpentry's teaching is hands-on, so participants are encouraged to use
their own computers to insure the proper setup of tools for an efficient
workflow.
*These lessons assume no prior knowledge of the skills or tools*, but working
through this lesson requires working copies of the software described below.
To most effectively use these materials, please make sure to install everything
*before* working through this lesson.

1. Create a github account if you do not have one already
  * Go to [github.com](https://github.com) and pick a username and password to create an account
2. For Windows users: Install git via https://git-scm.com/download/win
  * If you have never run git (you can check using `git config --list`) you need to set up your username and e-mail:
  * Either follow the detailed instruction on the [Software Carpentry](http://swcarpentry.github.io/git-novice/02-setup/) site or simply run:

  ```
  $ git config --global user.name "Your Username"  
  $ git config --global user.email "your@email.edu"  
  $ git config --global color.ui "auto"  
  ```

3. You should have a good text editor. [Atom](http://atom.io/) is a free an open source editor with excellent markdown support that we highly recommend you install and use, and some portions of this course rely on atom.
  * Atom is highly extensible with "packages" that add functionality. For markdown, install the package *Markdown Preview Plus*:
  * Click "Install a Package" or go to Edit --> Preferences (Atom -> Preferences on a mac) and click on "Install" on the left. Paste `markdown-preview-plus` into the search window, press return,  and click the blue "Install" button next to the package. On successful installation, you will have the package listed in the "Package" menu.
  * Paste `git-plus` into the search window, press return,  and click the blue "Install" button next to the package. (Not git-plus-plus) On successful installation, you will have the package listed in the "Package" menu.
  * If you do not want to install atom, many other good editors such as TextWrangler/BBEdit, Sublime, or Notepad++ work, too. There are also great online editors such as [hackmd](https://hackmd.io/), and [Dillinger](http://dillinger.io/) though we suggest you use a local tool here.
4. Optional: While we will default to git in atom / command line for this lesson,
consider installing the github desktop app from https://desktop.github.com/
