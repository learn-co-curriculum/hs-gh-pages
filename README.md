---
tags: kids, front end, gh-pages, deploy
languages: html, css
level: 1
type: Intro, Documentation
---

## Deploying with GitHub Pages

Now that you’ve got your site up and running it's time to deploy and share it with the world. This tutorial will walk you through how to use GitHub pages to publish your website.

### Initialize a new git repository in your project

You need to do this in order to track changes to your files and push up the latest version of your project to GitHub.

1. In your terminal, navigate to the root of your project (your main project directory - when you hit `ls` you should see your `index.html` file and `css` and `img` folders).

2. Initialize a git repository with `git init`. You only have to do this once at the very beginning of a project.

  Type `git status` to see the status of all your files. They should all be red because you have not staged them (prepared them) to be committed (frozen in time) and pushed up to GitHub (stored in the cloud).

3. Prepare your files to be committed with `git add .` Type `git status` again to see the status of your files - they should all be green and ready to go.

4. Commit your files with `git commit -m "commit message"`. The message can be anything you want, but it should be descriptive so that you'll remember the changes that are being captured in this version of the files. Your first commit can just be "initial commit".

### Set up a remote repository on GitHub
In order to publish your website you'll need to set up a repository on GitHub to store your project's files.

5. Log in to [GitHub](www.github.com). In the top right corner of the page you should see a plus sign that you can click on to create a new repository like this:

  ![img](https://s3.amazonaws.com/after-school-assets/new_github_repo.jpg)

6. Name the repository with the same name as your local directory. If this is the first site you are publishing with `gh-pages` you probably want to name it like this `<github username>.github.io`. GitHub has reserved this namespace for your own personal GitHub homepage.

  Keep it public, no need to add a README - click on "Create repository".

### Pushing up the work from your computer to GitHub

Now that you have a remote repository set up you just need to push up the work in the local directory on your computer up to the remote repository on GitHub.

7. When you created your GitHub repository you should have been redirected to a page for quick set up. Look for this section:

![img](https://s3.amazonaws.com/after-school-assets/connecting-remote-github-repo.png)

  Copy those two lines of code and paste them into your terminal. Hit enter to push up your code. Now go back to GitHub and refresh your page. You’ve got code!

### Creating a gh-pages branch
There is one other thing that we need to do before our work will be available to the public. In your terminal when you initialized your git repository you initialized it on a `master` branch. GitHub only publishes work that is on a `gh-pages` branch.

8. Type the following command into your terminal to create a new gh-pages branch: `git checkout -b gh-pages`

  The -b stands for branch. This command will create a new branch called gh-pages and checkout that branch - or move you onto that branch.

9. To push up your new gh-pages branch to GitHub type `git push origin gh-pages `

10. Go to GitHub and refresh the page. You should see a new branch available in the dropdown menu of branches.
![img](https://s3.amazonaws.com/after-school-assets/gh-pages-branch.png)

11. If you click on the repo settings - in the right nav bar - and scroll down to GitHub Pages you should see something like this:
![img](https://s3.amazonaws.com/after-school-assets/gh-pages-url.png)
With the url where you can see your published site.

## CONGRATS! You are published. Check out your site.

You are free to keep making changes to your site and you can publish them by committing your work - by adding, committing and pushing up with `git push origin gh-pages`.
