# How to setup git locally

A set of steps and configuration to get your git environment all setup.

```txt
# This is Git's per-user configuration file.
[user]
        name = <Your name>
        email = <email addres>
        signingkey = <signin key>
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
