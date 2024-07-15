install Git CLI
```
winget install --id GitHub.cli
```

1. Githu login

```
gh auth login
```

2. create a new repo and clone it to local

```
gh repo create readmeOne --public --clone
```

3. Clone a repo

```
gh repo clone repoName
```

4. push the updated code to GitHub

```
git push origin head: master
```

5. remote repo

check the remote repo

```
git remote -v
```

delete the remote repo

```
git remote remove origin
```

add a remote repo

```
git remote add origin https://github.com/Username/repoName.git
```

6. branch and merge

create a branch

```
git branch branchName
```

switch to the branch

```
git checkout branchName
```

merge branch

```
git merge branchName
```

check all branch

```
git branch -a
```
