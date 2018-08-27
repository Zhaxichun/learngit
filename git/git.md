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

### 3.1 add

### 3.2 commit

### 3.3 


    





