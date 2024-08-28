# How to setup git locally

```txt
# This is Git's per-user configuration file.
[user]
        name = Aaron East
        email = aaron@pactosystems.com 
        signingkey = 76F5FB6AE03B9477
[alias]
        a = add --all
        cl = clone
        br = branch
        ci = commit
        co = checkout
        st = status
        last = log -1 HEAD
        unstage = reset HEAD --
        glog = log --color --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit
        plog = log -p --color --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit
        slog = log --graph --oneline --decorate --all
[commit]
  template = ~/.gitmessage
[filter "lfs"]
        clean = git-lfs clean -- %f
        smudge = git-lfs smudge -- %f
        process = git-lfs filter-process
        required = true
[pull]
        rebase = true
[init]
        defaultBranch = main

```
