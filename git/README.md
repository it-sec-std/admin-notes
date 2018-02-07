## Submodules

Git Tools - Submodules

https://git-scm.com/book/en/v2/Git-Tools-Submodules


https://stackoverflow.com/questions/3796927/how-to-git-clone-including-submodules

`git clone --recursive -j8 git://github.com/foo/bar.git`


### Update all submodules

[Info from stof](https://stackoverflow.com/questions/1030169/easy-way-to-pull-latest-of-all-git-submodules)
`git pull --recurse-submodules`
if you want to pull your submodules to latest commits intead of what the repo points to.

Note: If that's the first time you checkout a repo you need to use --init first:

### Init all submodules

`git submodule update --init --recursive`

### Pull correct rev for all submodules

`git submodule foreach git pull origin master`

## Changing a remote's URL

https://help.github.com/articles/changing-a-remote-s-url/

```bash
git remote -v
git remote set-url origin https://github.com/USERNAME/REPOSITORY.git
```


## Recover data

I tend to use `git checkout .` which discards all changes from the working directory down. This makes a difference if you're not at the root of the repository.

# Duplicate git reps

https://help.github.com/articles/duplicating-a-repository/

```bash
Open Git Bash.

Create a bare clone of the repository.

git clone --bare https://github.com/exampleuser/old-repository.git
Mirror-push to the new repository.

cd old-repository.git
git push --mirror https://github.com/exampleuser/new-repository.git
Remove the temporary local repository you created in step 1.


cd ..
rm -rf old-repository.git
```

## Merging branch to master

https://stackoverflow.com/questions/5601931/best-and-safest-way-to-merge-a-git-branch-into-master

```bash
git checkout master
git pull origin master
git merge test
git push origin master
```
