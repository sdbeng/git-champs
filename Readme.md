## Git Champs - Practice git commands

## Instructions
You will be adding your first name to the list, specifically in the class.md file by making a pull request to my repo.

### Steps
- Fork my repo
- Clone it to your computer as you practice on class.
- In the command line, cd into that folder and open the class.md file
- Add your name in with an asterisk (*) like the ones already in the list.
- Since the best practices as a developer are to work on your local environment, you'll create your own feature branch in the command line. The purpose of having your own branch is to make your own contributions when you belong in a team or test a new feature, then later be merged in with the master.

Tip: always do `git status` to check up on a working clean directory or the current changes to be commited, if any. Don't forget often to `git pull` from the master to see latest changes.

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
Tip: you can run it on one line with `git commit -am 'message'`

- In order to push up your own branch to github, do:

```
git push -u origin jenns-update
```
- the -u option means upstream and origin is the name of the remote repo

Later, refresh the website, you should see your branch being pushed up to my github repo.

### Step 2
- Go to your github repo and create a Pull Request.

Later on my site, I'll integrate those branches into my master(if they're correctly made). 

Since I'm the one that created the repo, I will be the one with write permissions. 

So, this is pretty much what you'll do when working on a team if you are the designated member to compare and pull requests (PR).

This practice helped me a ton a while ago! The more you practice, the more you'll feel at home with git and be able to use it in all job / projects. I hope you all have fun! Can't wait to see your PRs!

## Tips
If you get stack, first research the output error and try to follow the proposed solution, sometimes it's just a command or two. Also look it up on Google, specifically on the Github help. Don't stress to much, this is not a homework:)





