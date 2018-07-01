## Git Champs - Practice git commands: Your first PR

## Instructions
You will be adding your first name to the list, specifically in the class.md file by making a pull request to my repo.

### Steps
- Do a `git pull` then fork my repo
- Clone it to your computer as you practice on class.
- In the command line, before making any local changes to go ahead and create your feature branch. See **Step1**
- Since the best practices as a developer are to work on your local environment, you'll create your own feature branch in the command line. The purpose of having your own branch is to make your own contributions when you belong in a team or test a new feature, then later be merged in with the master.
- Once you checked out in your branch, cd into that folder and open the class.md file
- Add your name in with an asterisk (*) like the ones already in the list.

Tip: always do `git status` to check up on a working clean directory or the current changes to be commited, if any. Don't forget to often do a `git pull` from the master to see latest changes. You never know when someone else has already made new contributions.

### Step 1
- In order to create your own branch do `git checkout -b name-of-your-branch`. 
- You'll automatically be switched into your own feature branch - Make sure to replace 'Jenn' with your own first name.
```
git status
git checkout -b jenns-update
```
- Then add and commit changes,
```
git status
git add --all
git commit -m "Jenn contributes to git-champs"
```
**Tip**: you can run one line command with `git commit -am 'message'`

- Next, In order to push up your own branch to github, do:

```
git push -u origin jenns-update
```
- the -u option means upstream and origin is the name of the remote repo

Go ahead refresh the github website, you should see your branch being pushed up to my github repo.

### Step 2
- Go to your github repo and create a Pull Request.

Later on my site, I'll integrate those branches into my master(if they're made correctly). 

Since I'm the one that created the repo(read & write access, I will be the one accepting the PR. 

This is pretty much what you'll do when working on a team if you are the designated member to compare and pull requests (PR) on a project.

**Note**: This practice helped me a ton a while ago! The more you practice, the more you'll feel at home with git and be able to use it in all jobs / projects where collaboration is key. I hope you all have fun! Can't wait to see your PRs!

## Tips
If you get stack, first research the output error and try to follow up the proposed solution, sometimes it's just a command or two. Also look it up on Google, specifically on the Github help. Don't stress to much, this is not homework:)

Changes made to Readme before rebase.

## Merge conflicts
Sometimes when the team inadvertently make changes to the working repo, you must to be ready to **reconcile** those changes. This comes into play when you try to pull out the code.

You'll first need to get rid of the unwanted lines of code, then add and commit to master.

Always check the logs with `git log` and also you can have a look at the HEAD by doing `git reflog`.

I strongly recommend to read the [docs](https://git-scm.com/docs/git-reflog) and practice by making simple changes to a repo.

One more important command is `git reset`.
`git reset --hard <commit>`
`git reset --hard origin/master`

They will help you go back in time and reset your code to the previous state, getting rid of code you don't want or it's not working.

