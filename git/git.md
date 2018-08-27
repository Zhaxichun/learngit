# use git to make version control.

## 1. Init local resp

### 1.1 Init a local resp:
~~~git
git init
~~~

### 1.2 Set signiture.
in order to differer code. have no bussiness with github.

> Attention: empty is forbidden.
> config info stored: current config: `.git/config`; global config: `~\.gitconfig`

there are one optional,`--global`

    ~~~git
    git config --global user.name xxx
    git config --global user.email xxx@xxx.xx
    ~~~
    Apply to current resp
    ~~~git
    git config --global user.name xxx
    git config --global user.email xxx@xxx.xx
    ~~~

If both are exsited, git will use the resp setting.

## 2. Local resp & remote resp

### 2.1 Communicaiton internally in team.

+ Remote resp (empty) - created by project initiator.
    * creator `push` local resp to remote resp.
    * team member `clone` remote resp to his/her local resp.
    * Team member do `push` to remote resp once do some change.
    * other team member do 'pull' to get update from remote resp.

### 2.2 Communication cross teams.

+ use `fork` to copy a remote resp of creator to my own remote resp.
    * `clone` the remote resp to local resp.
    * `push` changes to his own remote resp.
    * `pull request` --> review --> merge to original remote resp.

## 3. Command Line operation.
~~~
git status // find untrack files
add, commit, 
~~~

- git config
    - get help config
    - > dsk 
- git help
- **`git init`**
- `git add`
- git `clone`
- `git status`
- `git diff`
    - > To show the changes.
- `git commit`
    - > git commit main.py -m "this is main.py file commit mark use -m option"
    - >git commit -a -m "？？mark"  to run `add` & `commit` at a time.
- git reset
- git rm
- git mv
- `git branch`
    - > Create new Branch   `git branch branch_name`

    - > view all branches: `git branch`
    - >  Change to branch: `git checkout new_branch`
- `git checkout`
- git merge
- git mergetool
- `git log`
    - > to show the commit history
- git stash
- git tag
- `git fetch`
- `git push`
    - > to Push local repository to remote server.
    - > git push origin master
- `git pull`
    - > update local repository.
- `git remote`
- git describle
- git rebase

## some step to use git.

~~~conf

// init a new repository
git init

// ssh public key
ssh-keygen -t rsa -C 'zhaxichun@163.com'

// add remote repository.
git remote add origin git@gitee.com:zhaxi/leangit.git

[core]
    repositoryformatversion = 0
    filemode = false
    bare = false
    logallrefupdates = true
    symlinks = false
    ignorecase = true
[remote "origin"]
    url = git@github.com:hwangfantasy/beautify.git
    fetch = +refs/heads/*:refs/remotes/origin/*

# add new remote parameter.
[remote "mirror"] 
    url = git@git.oschina.net:hwangfantasy/beautify.git
    fetch = +refs/heads/*:refs/remotes/origin/*
[branch "master"]
    remote = origin
    remote = mirror # add info to branch info.
    merge = refs/heads/master
[gui]
    wmstate = normal
    geometry = 841x483+156+156 189 218

~~~


    





