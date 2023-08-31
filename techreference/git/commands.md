# Commands

## Branches

### Create

```
git branch <branchName>
```

#### Create and Switch in One

```
git switch -c <branchName>
```

#### Create Branch from Specific Commit ID

```
git branch <branchName> <commitID>
```

### Delete

```
git branch -d <branchName>
```

#### Force Delete

```
git branch -D <branchName>
```

### List

```
git branch
```

{% hint style="info" %}
A \* denotes the current branch
{% endhint %}

### Switch

```
git switch <branchName>
```

## Commit

### Commit Changes

```
git commit -m "Your brief message here"
```

### Log History

Verbose log of current branch

```
git log
```

Compact log of current branch

```
git log --oneline
```

Log of all commits in the repository displayed as graph

```
git log --oneline --all --graph
```

## Diff

### Branches

```
git diff <branchName1> <brancheName2> --
```

### Commits

```
git diff <commitId1> <commitId2> --
```

### General Options

#### By word not line

```
git diff --word-diff --
```

### Index and the object database

```
git diff --cached --
```

#### File in index and the object database

```
git diff --cached -- <fileName>
```

### Working directory and index

```
git diff --
```

#### File and that file in index

```
git diff -- <fileName>
```

## Files/Folder Tracking

### Add

#### All

```
git add -A
```

#### Specific Files

```
git add <fileORfolder1> <fileORfolder2> ...
```

### Restore

#### Index to working dir

```
git restore <fileORfolder1> <fileORfolder2> ...
```

#### Object DB to the index

```
git restore --staged <fileORfolder1> <fileORfolder2> ...
```

## Config

### List

```
git config -l
```

### Update

```
git config --global <key> <value>
```

## Help

### Man page style

```
git help <command>
```

### Short

```
git <command> -h
```

## Merge

Abort a merge attempt (only possible if there are conflicts)

```
git merge --abort
```

Merge a (feature) branch into the current (integration) branch

```
git merge <featureBrachName>
```

## Remove file or folder from index

```
git rm --cached <fileORfolder1>
```

## Status

### Long

```
git status
```

### Short

```
git status -s
```

Key/Legend

```
' ' = unmodified
M = modified
T = file type changed (regular file, symbolic link or submodule)
A = added
D = deleted
R = renamed
C = copied (if config option status.renames is set to "copies")
U = updated but unmerged

       X          Y     Meaning
       -------------------------------------------------
                [AMD]   not updated
       M        [ MTD]  updated in index
       T        [ MTD]  type changed in index
       A        [ MTD]  added to index
       D                deleted from index
       R        [ MTD]  renamed in index
       C        [ MTD]  copied in index
       [MTARC]          index and work tree matches
       [ MTARC]    M    work tree changed since index
       [ MTARC]    T    type changed in work tree since index
       [ MTARC]    D    deleted in work tree
                   R    renamed in work tree
                   C    copied in work tree
       -------------------------------------------------
       D           D    unmerged, both deleted
       A           U    unmerged, added by us
       U           D    unmerged, deleted by them
       U           A    unmerged, added by them
       D           U    unmerged, deleted by us
       A           A    unmerged, both added
       U           U    unmerged, both modified
       -------------------------------------------------
       ?           ?    untracked
       !           !    ignored
       -------------------------------------------------
```
