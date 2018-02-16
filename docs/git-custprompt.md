## Show current tracked branch

Open the Terminal app and if the file ~/.bash_profile does not already exist create it with the following command.

touch ~/.bash_profile

Open ~/.bash_profile in your favorite editor and add the following content to the bottom.
```
parse_git_branch() {
     git branch 2> /dev/null | sed -e '/^[^*]/d' -e 's/* \(.*\)/ (\1)/'
}
export PS1="\u@\h \[\033[32m\]\w\[\033[33m\]\$(parse_git_branch)\[\033[00m\] $ "
```
In here parse_git_branch() function extract the branch name when your are in git repository. This function output used in PS1 variable in order to prompt the branch name.

In above PS1 we defined following properties:
* \u@\h \[\033[32m\] - user, host name and its displaying color
* \w\[\033[33m\] - current working directory and its displaying color
* \$(parse_git_branch)\[\033[00m\] - git branch name and its displaying color

Now when you go to git repository form the terminal it will display currently checked out git branch in the prompt. Following is the example output of bash prompt after adding these changes to ~/.bash_profile

Finally, save the bash_profile:
```
source .bash_profile
```
Done.
