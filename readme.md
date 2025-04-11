# "version control"

# Annotated tags vs Lightweight Tags

## Annotated tags

```
 git tag -a "versionName" -m "message"

 -git show "versionName"
 -- That shows the tagger information, the date the commit was tagged, and the annotation message before showing the commit information.
```

## Lightweight Tags

```
 git tag "versionName"

 -git show "versionName"
 -- This time, if you run git show on the tag, you don’t see the extra tag information. The command just shows the commit:
```

## How to Remove Branches Locally and Remotely

### To delete a branch locally:

```
git branch -d branchName

```

### To delete a branch remotely:

```
git push origin --delete branchName

```

# Rebase

## When to use Rebase ?

```
* git-rebase - Reapply commits on top of another base tip *

1.To keep your commit history clean.
2.To make your branch up-to-date with the latest main without creating a merge commit.
( use git rebase main )
3.✅ If you and your teammate are working on the same branch and someone pushes before you, do:
( git pull --rebase )
```

# Tags

## How to list tags?

```
1. git tags ==> show all tags
2. git tag -l "v1.*" ==> List tags with a pattern
3.git show "tag-name" ==>List tags with commit information
4.git tag --sort=version:refname ==>List tags sorted by version
```

## How to delete tag locally and remotely?

### tag locally

```
git tag -d <tag-name>

```

### tag remotely

```
git push origin --delete tag v1.0.0

```

![My Image](image.jpg)
