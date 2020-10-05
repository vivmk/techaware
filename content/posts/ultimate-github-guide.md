---
title: "Your ultimate beginner guide to explore GitHub from scratch"
date: 2020-10-02T23:30:29+05:30
draft: false
author: "Vivek Mishra"
description: "This is for someone who has heard of GitHub somewhere, who knows little about what it is used for, or someone who tried it but found it hard work with or understand. Let us make this simple."
tags: ["Beginner", "General", "Career"]
---

#### What is it actually?

GitHub is a code hosting platform for version control and collaboration. It lets you and others work together on projects from anywhere.

#### Why so much fuss about it?

- Reason 1: **Immensely Powerful Community**
- Reason 2: **The Largest Shared Repository**
- Reason 3: **Easy Version Control**
- Reason 4: **A Myriad Of Integrations**
- Reason 5: **Secure Cloud Storage**

Hope those are enough reasons to get you started! :smile:

---

`Okay, get me started already!`

I will be focusing more on making this work on **Windows OS**. If you are on MacOS / Linux, things might be little different but not a lot. Anyways, things that you will need to start:

1. GitHub account - Create [here](https://github.com/).
2. Git Bash - Download [here](https://github.com/git-for-windows/git/releases/download/v2.28.0.windows.1/Git-2.28.0-64-bit.exe).

Let us have a look at the GitHub workflow now:

![GitHub workflow](https://hackernoon.com/hn-images/1*iHPPa72N11sBI_JSDEGxEA.png)

Do not worry if it looks scary to you now, at the end of this, you will master it.

### How and where do I start?

Follow these steps in given order:

1. [Create](https://docs.github.com/en/enterprise/2.13/user/articles/creating-a-new-repository) a GitHub repository. To avoid errors, do not initialize the new repository with _README_, license, or `gitignore` files. You can add these files after your project has been pushed to GitHub.

2. Open `Git Bash` and change the current working directory to your local project.

3. Initialize the local directory as a Git repository by running:

   ```bash
   $ git init
   ```

4. Add the files in your new local repository. Add the files in the local repository and stages them for commit using the command:

   ```bash
   $ git add .
   ```

5. Commit the files that you have staged in your local repository using:

   ```bash
   $ git commit -m "First commit"
   ```

6. At the top of your GitHub repository's Quick Setup page, click the copy icon of the remote repository URL as shown below:

   ![Copy the repository URL](https://docs.github.com/assets/images/help/repository/copy-remote-repository-url-quick-setup.png)

7. In the Command prompt, add the URL for the remote repository where your local repository will be pushed:

   ```bash
   $ git remote add origin https://github.com/your_username/your_reponame.git
   $ git remote -v
   ```

8. Push the changes in your local repository to GitHub:

   ```bash
   $ git push origin master
   ```

#### Hey! You just did your first work on your project!

Keep pushing your changes to the repository.

`Note:`
If you are working on [VS Code](https://code.visualstudio.com/download) editor, you can connect it directly to your repository using the menu option in the left side bar as described in the tutorial [here](https://code.visualstudio.com/docs/editor/github).

---

### Okay, done. What next?

Next is contributing to a project owned by someone else:

1. Go to the repository on GitHub.
2. Click the “Fork” button at the top right.
3. You will now have your own copy of that repository in your github account.
4. Open a Git Bash and type:

   ```bash
   $ git clone git@github.com:your_username/the_repo
   ```

5. You will now have a local copy of your version of that repository.
6. Change into that project directory (the_repo):

   ```bash
   $ cd the_repo
   ```

7. Add a connection to the original owner’s repository:

   ```bash
   $ git remote add owner_username git://github.com/owner_username/the_repo
   $ git remote -v
   ```

8. Run `git add` and `git commit` those changes.

9. Run `git push` to send them to GitHub. These will go to your version of the repository.

10. When you feel like submitting your changes to the main project of owner, click on `Compare & Pull Request` and send a request as shown:

    ![Pull Request](https://www.freecodecamp.org/news/content/images/2020/01/pullRequest-1.png)

---

### It was bit complicated right?

It is hard. It is always hard the first time you do something. Especially when you are collaborating, making mistakes is not a comfortable thing. But remember, it will be fun once you get used to it :wink:

`Eat, Sleep, Commit, Repeat !`
