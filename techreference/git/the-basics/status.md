# Status

## Commands

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
