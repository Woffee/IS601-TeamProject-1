## Remote Add 
To add a new remote Git repository as a shortname you can reference easily, run git remote add < shortname> < url>.


## Remote Remove
To remove a remote, navigate to the directory your repository is stored at, and use the git remote rm (or git remote remove) command followed by the remote name.

git remote rm <remote-name>

## Remote Show

Gives some information about the remote <name>.

With -n option, the remote heads are not queried first with git ls-remote < name>; cached information is used instead.
