# Branch

## Commands

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

### Fetch

Retrieves all remote branches without updating any local branches

```
git fetch
```

### Pull

```
git pull
```

### List

{% hint style="info" %}
A \* denotes the current branch
{% endhint %}

```
git branch
```

### Push

#### Remote Already Set

```
git push
```

#### Specify Remote

```
git push -u origin <branchName>
```

### Rename

#### Current Branch

```
git branch -m <newBranchName>
```

#### Specify  Branch

```
git branch -m <oldBranchName> <newBranchName>
```

### Switch

```
git switch <branchName
```
