# Searching

## Commands

### Blame

```
git blame <fileName>
```

#### Blame on a specific Commit ID

```
git blame <commitID> <fileName>
```

### Grep

Search the files that are tracked by the repo using a regex string.

```
git grep <searchString>
```

#### Case Insensitive

```
git grep -i <searchString>
```

#### Line Numbers

```
git grep -n <searchString>
```

#### Return Filename Only

```
git grep -l <searchString>
```
