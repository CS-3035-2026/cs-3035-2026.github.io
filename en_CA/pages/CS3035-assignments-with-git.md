# Using Git and GitHub

We will be using Git to access example code, fetch activities, and submit work on GitHub. Git is a very powerful tool, but the way we will use it for the course will be quite simple. In all cases, repositories will be created for you and you will "clone" the repositories to get started.

You will need to ensure [Git is installed](https://git-scm.com/downloads) and you have a working [GitHub account](https://github.com/join), if you don't already have one, to perform the steps below and to submit work in the course.

We ask that you follow these below carefully, and only stray from them if you know what you are doing.
There are lots of great git learning resources online, like the free [Pro Git Book](https://git-scm.com/book/en/v2), if you would like to learn more.

## Example Code

To access example code for the course, there is a repository setup on the course's [Github Example Repo](https://github.com/CS-3035-2026/examples). 

This repository will provide you with examples to get you started and provide additional context for topics we have covered in class. The code in the repository will grow and change over time, so you will want to regularly "pull" changes and new code so that you have the latest versions. You can also "watch" the repository by "starring" it on the GitHub website so that you can be notified of any changes.

**Remember** to pull the code from the examples repo often, as new examples will be added as the course progresses.

## Accessing the Class Repos

Each of the class's activities, examples, and projects will be hosted on Git Hub, and you will be provided with an invite link to each as they become available.

After accepting the invite to the repo in question, a fork (new copy) of that repo will be made for you to use.
For example, accepting ```https://github.com/CS-3035-2026/Project``` a new repo called ```https://github.com/CS-3035-2026/Project-YourUserName``` will be created for you. Only you and the course instructors and TAs will have access to your repos.

### Git and VS Code

We'll primarily use Git in VS Code and the integrated VS Code terminal environment.

To open your repo in **VS Code**, do the following:

- In the  ```Source Control``` tab of the sidebar, select ```Clone Repository```.
- In the bar now at the top of the window, select ```Clone from Github```.
- Enter the URL of the *your* version of the repo.
It should look like this: ```https://github.com/CS-3035-2026/RepoName-YourName.git```
- You will be asked where you'd like to clone this repo; this means where you would like to save the files locally on your computer while you work on them. It's highly recommended that you make a new folder for CS-3035 and then make a new folder inside that for each repo you work on.
- After selecting ```Open```, you will have the repo loaded into VS Code and available to work in.

## Preparing your repos

Once you have a repo open, a few steps are needed to get it ready to run and edit. These steps are terminal commands you'll need to do only once for each repo, but without doing them, the code will not be executed.

- SimpleKit is included in the project as a Git submodule. This means the SimpleKit repo is cloned into your project as a reference to its own repo, so you can access and use it, but if changes are made to the main SimpleKit repo, you can pull them directly without changing your project files.
- However, first, you must initialize the submodule and update the repo by running:
- ```git submodule init```
- ```git submodule update```
- If this doesn't work, you may need to read the submodule first by running the following:
- ```git submodule add https://github.com/CS-3035-2026/simplekit``` before running the above commands
- After this, SimpleKit will be ready to use. Next, you just have to install the NPM packages that have already been set up for you. Just run:
- ```npm install```
  
Once these steps are complete, you don't have to re-run them if you close and reopen the project.

### Running the Projects

Once the project is prepared, you can run the project by entering the following:

- ```npm run dev```
- or, by using the ```Run``` button in VS Code
  
This will activate the Vite module, which starts a local dev server and provides you with a 'LocalHost' web address, which you can paste into Chrome and view the project. The dev server will re-transpile as you make changes to the TypeScript files, but if you wish to stop the server, just press ```Q + Enter``` in the terminal.

## Activities

Activities will be hosted and submitted on GitHub. You will need to follow the instructions above to retrieve and submit them.

For convenience, we have also set up an example that will be your first in-class activity.

***Instructions*** will always be found in the repository's README.md file.

- For each activity, you will be provided a repository invitation link.
- You will follow the link, log in to GitHub (if you are not already logged in), and accept the invitation.
- This will create a new repository for you.
- A link will be provided for a repository that has been automatically created on your account
- Follow the link to view your repo
- Follow the instructions above to prepare and run the project.
- Now, you can edit the code and complete the activity.
- Once you have completed all of your changes, you need to commit to them.

Note: Before you can push your repo to GitHub, you will need to set your email and username for verification. You only need to do so once on any machine you use, and you can do so via these commands:

- ```git config --global user.email *your@githubemailaddress.com*```
- ```git config --global user.name *yourGithubUsername*```

Afterwards, you can proceed to commit and push your changes.

- To ***commit***:
  - First stage your changes in all files by typing ```git add .```
  - Once they are staged, you can ```git commit -m "message"```, in which *message* is replaced by a description of your changes, in quotes.
- Lastly, you can ***push*** your commits to GitHub to submit your assignment
  - type ```git push``` to update your GitHub repo with your new changes.
- Finally, visit your Repo on GitHub to make sure your changes have been pushed.

Here is the invitation link for the starter activity. (well, it will be soon)
