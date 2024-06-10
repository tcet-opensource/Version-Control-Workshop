<p align="center">
  <img src="https://github.com/tcet-opensource.png" alt="TCET Open Source Logo" width="200">
</p>

# TCET Open Source Git-GitHub Workshop

Welcome to the TCET Open Source Git-GitHub Workshop! 🚀

This repository is designed to help you get started with version control using Git and GitHub. Whether you're a beginner or looking to refresh your knowledge, we've got you covered.

> [!NOTE]
> # Why no PRs are merged?
> There are few reasons why no PRs are merged to the main branch
> ### Key Issues
> - Base Branch Mismatch: All the submitted PRs are created with the main branch as the base. While this is a common practice, it can lead to problems when multiple contributors are working on different features simultaneously.
> - Merge Conflicts: Due to the base branch mismatch, when a PR is merged, it can cause merge conflicts with other pending PRs. These conflicts occur because the main branch has changed since the other PRs were created, making it difficult or impossible to automatically merge the changes.
> ### Understanding the Problem
> - When you fork a repository and make changes in your local branch, you're working on a snapshot of the original repository at the time you forked it. Meanwhile, the original repository (upstream) continues to evolve as other contributors merge their changes.
> ## Here's what happens:
> - You fork the repository and create a branch based on the main branch.
> - You make changes and submit a PR to the original repository's main branch.
> - Before your PR is reviewed or merged, another PR gets merged into the main branch.
> - Now, your PR is based on an outdated version of the main branch, causing a merge conflict.
> ## Solution
> -  Keep Your Fork Updated: Regularly synchronize your fork with the upstream repository using `git pull upstream main`.
>   This ensures that your fork's main branch stays up-to-date with the latest changes.
> - Rebase Your Branch: Before submitting a PR or after updating your fork, rebase your feature branch onto the latest main:
>   ```bash
>   git checkout feature/your-branch
>   git rebase origin/main
>   ```
>   This applies your changes on top of the latest main, reducing the likelihood of merge conflicts.
> - Branch Management: Create a new branch for each feature, bug fix, or task you're working on.
>   Use descriptive branch names like `feature/add-login`, `bugfix/fix-memory-leak`, or `docs/update-readme`.
>   This keeps your changes isolated and makes it easier to manage conflicts.

## What is Git and GitHub?

**Git** is a distributed version control system that helps you track changes in your project's source code over time. It allows multiple contributors to collaborate on a project efficiently.

**GitHub** is a web-based platform that provides Git repository hosting, collaboration tools, and a community of developers to help manage your Git projects. It makes working with Git easier and more accessible.

## How to Get Started

1. **Fork this Repository**: Click the "Fork" button at the top right of this page to create your copy of the repository. This will allow you to make changes without affecting the original.

![image](https://github.com/Aisu2635/git-workshop/assets/104310687/d0dfcad9-4212-4021-8272-c2965d74c6cc)

2. **Clone your Fork**: After forking, open your forked repository and click the "Code" button. Copy the repository URL. Then, open your terminal and run the following command, replacing `[your-username]` with your GitHub username:

   ```bash
   git clone https://github.com/[your-username]/TCET-Open-Source-Workshop.git
   ```
**Commit Your Name**: Open the `name.html` file, and add your name to the list of contributors. Then, commit your changes with the following commands:
```bash
git add name.html
git commit -m "Added [Your Name] to the contributors"
git push
```
**Create a Pull Request**: Go back to your forked repository on GitHub, and you'll see a green "Compare & Pull Request" button. Click it to create a pull request to the original repository. Your contribution will be reviewed and merged!

## Open Source Contribution
We believe in the power of open source collaboration. By participating in this workshop, you're not only learning but also contributing to the global open source community. Every contribution counts!

## Resource
<p align="center">
  <a href="https://arsynthecatastrophe.notion.site/git-github-workshop-23f519477dae4f988783d0d63ed93853?pvs=4">
    <img src="https://img.shields.io/badge/Resource-📗-blue" alt="Resource" style="height: 50px">
  </a>
</p>



## Social Links

<div align="center">
<h3> Connect with us<a href="https://gifyu.com/image/Zy2f"><img src="https://github.com/milaan9/milaan9/blob/main/Handshake.gif" width="50px"></a>
</h3> 
<p align="center">
    <a href="https://twitter.com/tcetopensource" target="_blank"><img alt="Twitter" width="40px" src="https://www.iconpacks.net/icons/2/free-twitter-logo-icon-2429-thumb.png"></a> &nbsp&nbsp&nbsp
    <a href="https://www.instagram.com/tcetopensource/" target="_blank"><img alt="Instagram" width="40px" src="https://cdn-icons-png.flaticon.com/512/1384/1384063.png"></a> &nbsp&nbsp&nbsp
    <a href="https://discord.gg/r7ZhAREg2M" target="_blank"><img alt="Discord" width="40px" src="https://cdn-icons-png.flaticon.com/512/5968/5968756.png"></a> &nbsp&nbsp&nbsp
    <a href="mailto:opensource@tcetmumbai.in" target="_blank"><img alt="Gmail" width="40px" src="https://cdn-icons-png.flaticon.com/512/5968/5968534.png"></a> &nbsp&nbsp&nbsp 
    <a href="https://www.linkedin.com/company/tcet-opensource/" target="_blank"><img alt="LinkedIn" width="40px" src="https://cdn-icons-png.flaticon.com/512/3536/3536505.png"></a> &nbsp&nbsp&nbsp
</p> 

Happy coding and collaborating! 💻✨
