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

## Changing a remote's URL

https://help.github.com/articles/changing-a-remote-s-url/

```bash
git remote -v
git remote set-url origin https://github.com/USERNAME/REPOSITORY.git
```


## Recover data

I tend to use `git checkout .` which discards all changes from the working directory down. This makes a difference if you're not at the root of the repository.
