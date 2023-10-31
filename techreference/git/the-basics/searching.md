# Searching

## Commands

### Bisect

See the [Working with Bisect](../how-to/working-with-bisect.md) page.

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

### Log

Remember these flags can be used with other ones to manipulate the view.

#### Diff Text Search

Search for text in files

```
git log -G <searchString> (fileName)
```

#### Commit Search

```
git log --grep <searchString
```

#### Pickax Search

Search the commit log

```
git log -S <searchString> (fileName)
```

#### Patch

Show the diff between each commit.

```
git log -p
```

#### Patch Word Diff

Patch with the word difference in line.

```
git log -p --word-diff
```
