# Github Pages
30 Minutes

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
* Pick a theme (any theme will do -- pick your favorite!)
* **Tip**: Copy the URL of your website and edit the "description" on the "Code" tab of your github repository to include it so you can find it easily

### Downloand ("clone") the repository to your computer
* We do need the command line.
* Go to the "Code" tab of your repository
* Click on "Clone or download"
* Copy the HTTPS link for your repository
* In the Terminal (or on git bash on Windows), navigate to the folder where you would like to work. You may need to create that folder first e.g.
```
cd ~/Desktop
mkdir resume-website
cd resume-website
```
* Now "clone" the repository from github using
```
git clone https://github.com/<yourgithubusername>/my-first-webpage.git
```
* In Atom, using the "Open Folder" command under "File", open the resume-website folder you just created.
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






Previous: [Markdown Syntax](01-markdown-syntax.html)  Next: [Setting up Jekyll](03-jekyll-setup.html)
