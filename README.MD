This repository is an example of how we can work on multiple branches without the need of **checkout** between them using **WORKTREES**.

# How?
Suppose you are checked in **master** branch and you want to work on another branch called **fix** to add some changes.

Here's the initial state of your working directory:

![image](https://user-images.githubusercontent.com/19434305/114986369-96fa3980-9e9c-11eb-89ae-865c2086a305.png)

To create a worktree, use the following command: `git worktree add <folder-name> <branch-name>`

In our case, we will execute: `git worktree add hotfix fix`

A new folder will be added and it will reference the branch we passed.

![image](https://user-images.githubusercontent.com/19434305/114987292-aded5b80-9e9d-11eb-8873-5d9a8daf3ebd.png)

If you execute `git branch` inside **hotfix** folder, you will notice that the branch **fix** is checked in

![image](https://user-images.githubusercontent.com/19434305/114987884-58fe1500-9e9e-11eb-9e6a-ceed5915ddf4.png)

You can now add your changes to fix branch, commit, and push them and in the same time you can work on any other branch in the same way.



## Reference:

https://www.youtube.com/watch?v=qKCHSOQYRQI

## Git documentation for worktree:
https://git-scm.com/docs/git-worktree
