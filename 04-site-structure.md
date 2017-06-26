# Site Structure, Navigation, and Theming
?? minutes

## Learning Objectives

* Create several pages with some navigation and crosslinks
* Create an image folder and insert an image into your website
* Change your site's theme

---

## Site structure

Conveniently, Jekyll just uses the folder structure you create locally as the structure for your website.
* You can create pages and sub-pages simply by using folders. E.g. if you would like a page to talk about your hobbies with sub-pages basketball, painting, and salsa dancing, you would simply create `hobbies.md` in your website folder, create a new folder `hobbies` and in it create `basketball.md`, `painting.md`, and `salsa.md`. You would then have URLs like `<mypage>.github.io/hobbies/salsa`
  * **Tip**: You can do all of this in your file browser, but you can also stay entirely in Atom. By right clicking on your website folder on the left, you can create a new folder, and right-clicking on that folder lets you create files in that folder.

### Exercise
You now want to provide information about your dissertation research to your page. Create a page "Dissertation" that links to  sub-pages for Chapter 1, Chapter 2, Chapter 3 (or any other divisions you would like). Don't worry about populating any of those pages.

### Solution
* Right-click on the top-level folder, "my-first-webpage" on the left and select "New File". Create `dissertation.md` and add a YAML header (see below) and save the file.
```
---
title: Dissertation
layout: default
---
```
* Right-click again on `my-first-webpage` on the left, now select "New Folder and create `dissertation`.
* Right-click now on `dissertation` on the left, select "New File", create `chapter1.md` add a YAML header like the one above and save.
* Proceed alike for chapters 2 and 3.
* Now open up `dissertation.md` and create links to these three chapters. That be something like
```
Learn more about my dissertation.
* Details about chapter 1 are [here][dissertation/chapter1]
* Details about chapter 2 are [here][dissertation/chapter2]
* Details about chapter 3 are [here][dissertation/chapter3]
```
* Use "Add all, commit, and push" to push your changes to github and see your results.

Previous: [Jekyll Setup](03-jekyll-setup.html)  Next: [Changing Your Site Theme](05-changing-theme.html)
