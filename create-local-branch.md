### Create a local repo and push it to github - Step by step

```
git init
git add -A
git commit -m 'First commit'
```
- Go to github.com, create a new repo(don't add anything), copy the [url] provided, i.e. [https://github.com/your-username/repo-name.git]
* Then, you're need to add a remote to your local master branch
```
git remote add origin [url]
```
* Finally, push your master branch to the remote origin:
```
$ git push -u origin master
```
- Go to github.com and refresh the website 👏