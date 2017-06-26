# Github Pages
40 Minutes

## Learning Objectives
* Set up a github repository for a webpage
* clone the repository to your computer
* make local changes and push them to your github site.

----------------------------------------------------

## Lesson

### Start a repository for the page on github

* Go to https://github.com and  log in with your account
* Click on "Start a project"
* Pick a (short) name, e.g. my-first-webpage; add a description if you'd like; leave the site public
* Check the "Initialize with Readme" option. Under "Add .gitignore" choose "Jekyll"
* Click "Create repository" to do just that

### Set up the page on github
* Your new repository will open on github
* Click on "Settings" at the top
* Under GitHub Pages, towards the bottom of the screen select "master branch" and click "Save".
  * **Quick Challenge**: github lets you choose between the master branch or a "Doc folder" within that branch. When would you consider choosing the Doc folder?
  * *Solution* The Doc folder is particularly useful when you are writing documentation to a project. That way, you can keep the code in the master branch and have the documentation in a subfolder.
* **Tip**: Copy the URL of your website and edit the "description" on the "Code" tab of your github repository to include it so you can find it easily later on:
  * After you set the source for your website, the URL will appear in green right above it. It will have the format \<yourgithubusername\>/github.io/my-first-webpage
  * Copy that URL. Then press the "Code" tab at the top of that page to get back to the root page of your repository.
  * Click on the green Edit button at the top right, next to "*No description, website, or topics provided*" and add your website URL in the "*Website for this repository*" field and click Save.
* Go back to the settings by clicking on the "Settings" tab at the top and scroll down to the "GitHub Pages" section again.
* Now pick a theme (any theme will do -- pick your favorite!):
  * You can click on the themes at the top and see a preview below
  * Click "Select Theme" to pick your favorite theme
  * GitHub will open the "README.md" with some prepopulated text.
* Remove the sample text from the README by clicking anywhere in the edit window, select all (`ctrl/cmd + a`) and the delete or backspace key.
* Scroll to the bottom of the screen to "commit" your changes. You can just use the default settings and press the green "Commit changes" button.

### Downloand ("clone") the repository to your computer
*We will need the command line here, so open terminal (Linux/Mac) or git bash (Windows)*
* Go back to the "Code" tab of your repository by clicking on "Code" at the top.
* Click on "Clone or download"
* Copy the HTTPS link for your repository
  * If you have SSH activated for github, use the SSH link instead.
* In the Terminal (or on git bash on Windows), navigate to the location where you want to put your repository. Desktop is a easy choice.
```
cd ~/Desktop
```
* Now "clone" the repository from github using
```
git clone https://github.com/<yourgithubusername>/my-first-webpage.git
```
(the URI will look slightly different using SSH, but the git clone command works exactly the same)
* In Atom, using the "Open Folder" command under "File", open your my-first-webpage repository.
* You should see 3 files on your left: `.gitignore`, `README.md`, and `_config.yml`

### Configuring your page
* Open `_config.yml` by clicking on it. This file contains basic information about your site.
  * `.yml` files are called "YAML" files.
* Change `title:` to something sensible like `title: John Doe's Homepage`
* Add a description using the `description:` tag.
* Save the configuration file (you can use `ctrl+s`)
* Open README.md by clicking on it on the left. This is going to be your homepage.
* You first need to add a "YAML header" at the top of the file. use

```
---
title: John Doe's Homepage
layout: default
---
```

* Then add some simple content such as

```
# John Doe's Homepage
You can find my Resume [here](/myresume.md)
```

* For now, just put any address in the link. We will add the link to your resume shortly.
* Save the file
* Now, in the "Package" menu of Atom, under git-plus, use the "add all, commit and push option"
* Make sure there are no errors, then check out your new website! It will be at https://<yourgithubusername>.github.io/my-first-webpage
* Take a moment to pat yourself on the back.

## Excercise
Can you figure out how to add the resume from the last topic as a separate page on the website?
What is its link? Can you change the link from the homepage so it links to it?

### Solution
* First copy your myresume.md file to the my-first-webpage folder
* Add a YAML header just like above, except with a different title.
* Run the add all, commit and push option
* Your resume will be on https://<yourgithubusername>.github.io/my-resume
  * Note the absence of the .md file extension. github/jekyll converts the file to an .html file, so the link also works ending in `my-resume.html`.






Previous: [Markdown Syntax](01-markdown-syntax.html)  Next: [Setting up Jekyll](03-jekyll-setup.html)
