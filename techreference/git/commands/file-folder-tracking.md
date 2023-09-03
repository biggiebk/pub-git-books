# File/Folder Tracking

## Commands

### Add

#### All

```
git add -A
```

#### Specific Files

```
git add <fileORfolder1> <fileORfolder2> ...
```

### Delete

#### File

```
git rm <fileName1> <fileName2>
```

#### Folder

```
git rm -r <folderName1>
```

#### If you did non git rm/delete

```
git add -u <fileName1> <fileName2>
```

#### From index

```
git rm --cached <fileORfolder1>
```

### Rename

```
git mv -u <oldFileName> <newFileName>
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
