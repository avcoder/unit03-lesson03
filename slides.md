---
# You can also start simply with 'default'
theme: default
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: /assets/intro.jpg
# some information about your slides (markdown enabled)
title: Software Development | Foundations
info: |
  ## Software Development | Foundations
# apply unocss classes to the current slide
class: text-left
drawings:
  persist: false
transition: slide-left
mdc: true
---

# Node.js - part 3/12
Back-End Development
- [ ] Git fundamentals: initializing a repo, commit, branch
- [ ] Use GitHub to host repositories and collaborate
- [ ] Collaborate on a shared web development project using git and GitHub

<div class="abs-br m-6 text-xl">
  <a href="https://github.com/slidevjs/slidev" target="_blank" class="slidev-icon-btn">
    <carbon:logo-github />
  </a>
</div>

<!--
TODO: fill in anchor href above to point to github repo for these slides
-->

---
transition: slide-left
---

# Git
(10 min) Install git; Create a local repo and commit changes

- What are some challenges of managing code without version control?
   - Ever lost code or overwritten files accidentally?
- How does VCS help in tracking changes and collaborating?
- Git is a distributed version control system (VCS)
   - Distributed: everyone can have a local copy of the repository
- What are benefits of using git?
   - Manage changes to source code over time, allows branching
   - Prevents losing work, tracks changes, enables collaboration
   - [Configure](https://www.freecodecamp.org/news/guide-to-git-github-for-beginners-and-experienced-devs#how-to-configure-git) global settings: username and email

<!--
-->

---
transition: slide-left
---

# Exercise: Initializing a Repository
(30 min) 

- Create a new project using a simple index.html and index.js
- Demo `git`:  `init` `add` `commit` `status` `log` (`push` `pull` to/from GitHub)
- Note: `.git` `.gitignore`
1. make a change in index.html, save - what happens?
1. stage > commit > push 

- Oops! How can I get back to a previous commit?
- Oops again! How can I go forward to the most recent commit?

<!--
-->

---
transition: slide-left
---

# Git Branching and Merging
(30 min) What are branches? Why do we use them?

- Demo `git`:  `branch` `checkout` `switch` `merge`
1. Create a new branch `git branch feature/ticket01/add-user-auth`
1. Switch to the new branch `git checkout feature/ticket01/add-user-auth` or use `switch`
1. Make changes and commit on that branch
1. Switch back to main branch `git checkout main` or `git switch main`
1. Merge changes `git merge feature/ticket01/add-user-auth`

<!--
-->

---
layout: image-right
transition: slide-left
image: /assets/primeagen.png
backgroundSize: 500px 80px
class: text-left
---

# 10 minute break

🍦 Cool Tips, Trends and Resources:

- ▶️ [Git and GitHub Crash Course 2025](https://www.youtube.com/watch?v=vA5TTz6BXhY)
- 🐺[The Git Parable](https://tom.preston-werner.com/2009/05/19/the-git-parable.html)
- 📈 [Git Graph](https://marketplace.visualstudio.com/items?itemName=mhutchie.git-graph)
- 🎲 [Git Cheat sheet](https://github.com/arslanbilal/git-cheat-sheet)
- 🎒 [Github Student Dev Pack](https://education.github.com/pack)

<br>
<hr>
<br>

- 🧪 [Enter anonymous lab questions](https://docs.google.com/forms/d/e/1FAIpQLSevvGARdHQikso-uLqFCO481MABKE5HofuSrlzEPMNQ2ZLykw/viewform?usp=dialog)
- ℹ️ [Course feedback survey](https://circuitstream.typeform.com/to/ZoyYk7px#course_id=SoftwareAN&instructor=9514)

<!-- 
- take attendance
-->

---
transition: slide-left
---

# GitHub
(40 min) Fork a repo, create a pull request

- GitHub is a platform for hosting git repositories allowing social collaboration
- ChatGPT: List popular open-source projects on GitHub that a beginner web developer might recognize regarding javascript, node, or css frameworks

- Exercises: 
   - Create a remote repository on GitHub
   - Link an already existing local repository to GitHub
   - Fork my "MadLibs" repo, clone it, make a change, and create a PR (Pull Request)

<!--
-->

---
transition: slide-left
---

# Exercise
Build a multi-page website collaboratively.

- Fork and clone my GitHub repo [collaborative-website](https://github.com/avcoder/collaborative-website/tree/main)
- Add to the story.  Put your name in the caption.
- Commit and create a PR, and I will merge your pull request
- View changes on production site: https://story123.netlify.app/

---
transition: slide-left
---

# Homework

- Play [Learn Git Branching](https://learngitbranching.js.org/)
- [Learn Git Basics](https://www.freecodecamp.org/news/learn-git-basics/)