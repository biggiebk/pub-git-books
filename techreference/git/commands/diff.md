# Diff

## Commands

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
