# Personal & Professional Websites w/ GitHub Pages

## ![CIDR](assets/cidr.240x140.png)

## https://sul-cidr.github.io/gh-pages-2021/

---

> This workshop will introduce you to using the free GitHub Pages service to host website and web pages online.
>
> We will take you through creating a GitHub account and a GitHub Pages site, and then show you how to create simple but useful web pages you can use to create an online presence for yourself or for a project or team.
>
> No prior experience is assumed or expected, and no special tools or software is required.

---

### Before we begin...

Please sign in for this workshop at:  
https://signin.cidr.link/Websites_with_GitHub_Pages/ <!-- .element: target="signin" -->

When you've submitted the sign-in form, please keep the browser tab open on the evaluation form as a reminder to complete it when the workshop is over.

---

### Overview

<ul>
  <li class="fragment">
    Websites and Web Pages
    <ul>
      <li>HTML, CSS, and JavaScript</li>
      <li>Static Sites vs. Dynamic Sites</li>
    </ul>
  </li>

  <li class="fragment">
    Git, GitHub, and GitHub Pages
    <ul>
      <li>Concepts and Services</li>
      <li>Creating a GitHub Account</li>
    </ul>
  </li>
  <li class="fragment">
    Writing and publishing HTML pages
    <ul>
      <li>Publishing from GitHub Pages</li>
      <li>A Self-Contained Web Page</li>
      <li>A Single-Page Résumé Site</li>
    </ul>    
  </li>
  <li class="fragment">Static Site Generators, Markdown, and Templating</li>
</ul>

---

<!-- .slide: data-background-image="assets/html-css-javascript.png" -->
<!-- .slide: data-background-size="100vmin" -->
<!-- .slide: data-background-position="right" -->
<!-- .slide: data-background-opacity="0.2" -->

### HTML, CSS, and Modern Web Pages

- The anatomy of a web page:
  - Content Layer (HTML)
  - Presentation Layer (CSS)
  - Behaviour Layer  
    (ECMAScript, more commonly known as JavaScript)
  - Other resources (images, media etc., potentially data)
- "Static" by nature
  - Clients (web browsers) download the resources  
    and render the page on the user's computer

---

### Static vs Dynamic Websites

- **Dynamic Websites**

  - A web application creates the resources (HTML) on-demand, when a user request is made
  - Typically (though not always) involve a database server
  - Can be updated in real time, while running
  - Examples include CMSs such as WordPress, Drupal, MediaWiki

- **Static Sites**

  - Resources are created in advance of user requests and are delivered to users exactly as stored
  - Updates require that some or all of the pages are modified/replaced/recreated
  - No special server-side software required
  - Resources can be created by a Static-Site Generator

:::
Dynamic sites involve running a some software (PHP, Python, Ruby etc.) on a server somewhere

---

### Advantages of Static Sites (I)

- Security
  - Fewer (or essentially no) moving parts mean an almost non-existent attack surface

<!-- .element class="fragment" -->

- Ease of Hosting
  - The simplest possible hosting requirements mean the site can be hosted almost anywhere  
    and at little to no cost

<!-- .element class="fragment" -->

- Ease of Maintenance
  - Nothing needs regular maintenance, security patching, etc.

<!-- .element class="fragment" -->

---

### Advantages of Static Sites (II)

- Portability and Preservation/Archiving
  - Static sites are trivial to backup, to move to new locations, and to put under version control

<!-- .element class="fragment" -->

- Speed and Scalability
  - The simplicity with which static sites can be hosted also means that pages can be served  
    as fast as they can be requested

<!-- .element class="fragment" -->

- Simplicity and Control
  - With fewer moving parts and less technology between the author and final page, it's easier  
    to feel a sense of ownership and control

<!-- .element class="fragment" -->

:::

- Static sites also _require_ the author to think more in terms of simplicity which generally results in better sites (for most of the above reasons)

---

### Disadvantages of Static Sites

- Some things are more difficult and/or require third-party services and solutions
  - Site search
  - Commenting

<!-- .element class="fragment" -->

- Some things just require dynamic content
  - User-specific content
  - Working with large datasets

<!-- .element class="fragment" -->

:::
say something about widgets?

- interactive elements
- maps

---

### Static Site Generators

- The principle behind SSGs is to separate content and layout/styling ("themes")
  - This has the major advantage of avoiding repetition
- Typically content is created in Markdown files
- The SSG combines the content files with a template to create the static HTML  
  (and CSS, JavaScript etc.) files which comprise the static site
- Popular SSGs include Gatsby, Hugo, Eleventy, and Jekyll

:::

---

## ![git](assets/git.png) <!-- .element class="logo-heading" -->

## ![GitHub](assets/github.png) <!-- .element class="logo-heading" -->

## ![GitHub](assets/github-pages.png) <!-- .element class="logo-heading" -->

---

<!-- .slide: data-background-image="assets/git.png" -->
<!-- .slide: data-background-size="100vmin" -->
<!-- .slide: data-background-position="bottom" -->
<!-- .slide: data-background-opacity="0.2" -->

<div class="r-stack">
  <div>
    <h3>git</h3>
    <ul>
      <li>Distributed Revision Control System</li>
      <li>Created by Linus Torvalds to support Linux kernel development in 2005</li>
      <li>Completely free and open-source (GPL-2.0-only)</li>
      <li>Has a reputation for being kinda gnarly</li>
    </ul>
  </div>
  <a href="https://xkcd.com/1597/" title="XKCD - Git" target="xkcd" class="fragment"><img src="//imgs.xkcd.com/comics/git.png" title="If that doesn't fix it, git.txt contains the phone number of a friend of mine who understands git. Just wait through a few minutes of 'It's really pretty simple, just think of branches as...' and eventually you'll learn the commands that will fix everything." alt="Git" srcset="//imgs.xkcd.com/comics/git_2x.png 2x"></a>
</div>
---

<!-- .slide: data-background-image="assets/git.png" -->
<!-- .slide: data-background-size="100vmin" -->
<!-- .slide: data-background-position="bottom" -->
<!-- .slide: data-background-opacity="0.2" -->

### Some git concepts

- **Repositories**

  - For our purposes, a repository (repo) is a collection of source files that are tracked under version control.
  - Repositories can be (are) distributed -- meaning that multiple copies can exist in multiple locations

- **Commits**
  - A collection of content representing the state of the repo at a given point
  - Are annotated with commit messages, which typically (should) describe the changes represented by the commit

<p class="notes">Note: This is heavily simplified and omits several important concepts needed to use git effectively on your local computer.</p>

:::
This is some notes.

---

<!-- .slide: data-background-image="assets/github.png" -->
<!-- .slide: data-background-size="100vmin" -->
<!-- .slide: data-background-position="bottom" -->
<!-- .slide: data-background-opacity="0.2" -->

### GitHub

- Repo hosting and additional services based around git
  - Regular remote git commands
  - Issues, PRs, Wikis, GitHub Actions (CI/CD), and much more
  - GitHub Pages
- Launched in 2008, it was acquired by Microsoft in 2018
- Provides free and premium services
- At time of writing, GitHub claims [> 60 million users](https://github.com/search?q=type:user&type=Users) and [~240 million repositories](https://github.com/search)

---

<!-- .slide: data-background-image="assets/github-pages.png" -->
<!-- .slide: data-background-size="100vmin" -->
<!-- .slide: data-background-position="bottom" -->
<!-- .slide: data-background-opacity="0.2" -->

### GitHub Pages

- Offers free static web hosting for public repositories
- Provides addresses of the form `<gh-user>.github.io/repo`
  - but can use custom domain names purchased and registered elsewhere
- Automatically creates free TLS (https) encryption certificates

---

### Limits and Limitations of GitHub Pages

- Static sites only!

- Maximum file size: 100 MB
- Maximum site size: 1 GB
- Bandwidth limit: 100 GB / month (soft limit)
- Build limit: **<mark>10 builds / hour</mark>** (soft limit)

- Public sites and repositories only (on free plans)

---

### Creating a GitHub Account

- Navigate to [github.com](https://github.com/) <!-- .element: target="github" --> and create an account

  - Enter the email address you want to use and choose a password
  - Complete the email verification process
  - "Skip Personalization" for now

- Let's complete the `README.md` repo

---

### Let's create some websites!

---

### Create a Repository

- Create a new repository with the name `<gh-user>.github.io`
  - if you already have a repo with this name, create a new repo with whatever name you like, but be ready to make changes later on

---

### The Simplest Possible Web Page

Copy-and-paste this simplest possible HTML document over the top of the `index.html` in your repo, and change the text. Commit the new version, and wait for GH-Pages to deploy your new page.

```html [1|2-4|5-8|9|1-9]
<html>
  <head>
    <title>Your title here...</title>
  </head>

  <body>
    Your content here...
  </body>
</html>
```

---

### A Single-File Example

Let's create a more interesting example.

- Open the example page and take a quick look
  - https://simonwiles.github.io/gh-pages-2021/templates/one-file.html <!-- .element: target="one-file" -->
- Use <kbd>Ctrl</kbd> + <kbd>U</kbd> / <kbd>⌘</kbd> + <kbd>U</kbd> to "View Source" and take a look at the HTML
- Copy-and-paste the entire contents over the top of your `index.html` in your repository

---

### A One-Page Résumé Site

- Check out the example
  - https://simonwiles.github.io/gh-pages-2021/templates/one-page-resume/ <!-- .element: target="one-page-resume" -->
- Copy the page again, as before

---

### Some editing tricks

- github.dev
- Browser dev tools

---

### Markdown and Static Site Generators

Templating -- separation of content from layout/styling etc.
What to say about Jekyll? Hugo...
Developing locally

---

### Working with local files

---

### Further Resources

- HTML / CSS

  - https://www.w3schools.com/
  - http://www.csszengarden.com/

- GitHub Pages / Jekyll

  - https://programminghistorian.org/en/lessons/building-static-sites-with-jekyll-github-pages
  - https://programminghistorian.org/en/lessons/collaborative-blog-with-jekyll-github

- https://pages.github.com/

- https://jayrobwilliams.com/posts/2020/06/academic-website/

---

### Thanks!

Please fill out the evaluation form for this workshop at:
https://evaluation.cidr.link/Websites_with_GitHub_Pages/ <!-- .element: target="signin" -->

---
