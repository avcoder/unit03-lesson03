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

# Intro to Git
(10 min) 

- **Have you ever lost work or accidentally overwritten a file (especially in a group project)?**
   - How did you keep track of changes in your group project?
- Git is a distributed version control system (VCS)
   - Distributed: everyone can have a local copy of the repository
   - Differs from centralized VCS like SVN
- What are benefits of using git?
   - resolves issues like overwriting files, or losing changes
   - manages changes to source code over time
   - manages different version of a project through branching and merging
- Setting up Git for [first time](https://www.freecodecamp.org/news/learn-git-basics/#heading-how-to-configure-your-identity-in-git)

<!--
-->

---
transition: slide-left
---

# Exercise: Create repo, stage and commit changes
(20 min) Install VS Code extension "Git Graph" to help us visualize what's happening

1. Create a New Project Directory `mkdir my_proj` and navigate into it `cd my_proj` 
1. Initialize Git via `git init`
1. Create a simple index.html file: `<p>Once upon a time...</p>`
1. Run `git status` - What 4 pieces of info does it give?
1. To track/stage changes: `git add index.html` - How does `git status` compare now?
1. Commit changes: `git commit -m "add intro to fairy tale"`
   - How does `git status` compare now?
1. To view commit history, run `git log`
   - How does what `git log` outputs compare to when you `Cmd + Shift + P` and search/select "Git Graph: View Git Graph" 
   - (To quit the terminal screen, you may have to press 'q')
1. Discuss: What does `git add` and `git commit` do?

<!--
-->

---
transition: slide-left
---

# Exercise: Git Branching and Merging
(20 min) Make sure to run `git status` after each step to help visualize what's happening
 
1. Create a branch `git branch add-chapter-2`
1. Switch to the newly created branch `git checkout add-chapter-2` or `git switch add-chapter-2`
1. Edit `index.html` by adding more to "Once upon a time..." and save it.
1. At this point even though we could `git add .` or `git add index.html`, run `git add -p`
   - What info is git conveying? What do those different options mean after "Stage this hunk"?
   - Go ahead and press `y` then press enter, to stage our change 
1. Go ahead and commit our staged change `git commit -m "add next sentence"`
1. (Confirm index.html does indeed contain your latest change before moving onto next step)
1. Switch back to the main branch `git checkout main` or `git switch main`
   - Does index.html still contain your changes? 
1. `git branch -a` shows a listing of all branches; Do you see your branch there?
1. Let's merge that branch now via `git merge chapter-2`
1. Discuss: What happened when the feature branch was merged? Why is branching important?

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
- 🧑‍💻 [Hacktoberfest Beginner Resources](https://hacktoberfest.com/participation/#beginner-resources)

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
(5 min) GitHub as a platform for hosting Git repositories

- GitHub is a platform for hosting git repositories.  It allows:
   - [collaboration](https://github.com/facebook/react/pull/32813)
   - [track issues](https://github.com/facebook/react/issues)
   - contribute to [open-source software](https://www.freecodecamp.org/news/how-to-contribute-to-open-source-handbook/)
- Ask ChatGPT: 
   - List 10 popular open-source projects on GitHub
   - List 10 of the most popular GitHub repositories
- Check: Ensure you have a GitHub account

<!--
-->

---
transition: slide-left
---

# Exercise
(30 mins) Build a multi-page website collaboratively. Run `git status` after each step to help visually know

- Goto: [collaborative-website](https://github.com/avcoder/collaborative-website)
- in upper right corner, click "Fork" to fork the repo -- this makes a copy to your GH
- Download a copy to your computer: `git clone [insert url of your forked repo]`
- Create a branch `git checkout -b student1` or `git branch student1`
- Add your new HTML page (create your own story similar to index.html)
- Update the index.html to link to your new html page, (ensure it works locally)
- Commit your changes via `git add .` and `git commit -m "add student1 story"
- Push your changes to your forked repo on GH `git push origin student1`
- Create a Pull Request (PR): Go to your GitHub forked repo and create a PR from your branch (student1) to the main repo (collaborative-website)
- View changes on production site: https://story123.netlify.app/

---
transition: slide-left
---

# Exercise: Review and Merging PRs
(remainder of time) Continuing building a multi-page website collaboratively.

- Let's review each PR (check for any merge conflicts, naming oddities, etc)
- Discuss any improvements or suggestions
- I will merge each PR into my main branch of the repo 
- Check production website aka [prod](https://story123.netlify.app/) to test if new changes works


---
transition: slide-left
---

# Homework

- Assignment 2 due Apr. 13 Midnight EST
- Play [Learn Git Branching](https://learngitbranching.js.org/)