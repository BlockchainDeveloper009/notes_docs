md_git_commands.md


### error`: gitlog
-------------
```
git config --global user.email "you@example.com"
  git config --global user.name "Your Name"

to set your account's default identity.
Omit --global to set the identity only in this repository.

fatal: no name was given and auto-detection is disabled
2025-08-14 11:26:08.021 [info] > git config --get-all user.name [18ms]
2025-08-14 11:26:08.215 [info] > git config --get commit.template [98ms]
2025-08-14 11:26:08.242 [info] > git for-each-ref --format=%(refname)%00%(upstream:short)%00%(objectname)%00%(upstream:track)%00%(upstream:remotename)%00%(upstream:remoteref) refs/heads/devbr refs/remotes/devbr [36ms]
2025-08-14 11:26:08.359 [warning] [Git][revParse] Unable to read file: ENOENT: no such file or directory, open '/home/harishgk/source/repos/notes_docs/.git/refs/remotes/origin/devbr'
2025-08-14 11:26:08.403 [info] > git rev-parse refs/remotes/origin/devbr [45ms]
2025-08-14 11:26:08.596 [info] > git status -z -uall [92ms]
2025-08-14 11:26:08.617 [info] > git for-each-ref --sort -committerdate --format %(refname)%00%(objectname)%00%(*objectname) [25ms]

```