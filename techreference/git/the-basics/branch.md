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

Local

```
git branch -d <branchName>
```

#### Force Delete Local

```
git branch -D <branchName>
```

#### Remote Delete

```
git push -d origin <branchName>
```

### Fetch

Retrieves all remote branches without updating any local branches

{% hint style="info" %}
If you want to have the remote branch on the local one you need to merge after the fetch.
{% endhint %}

```
git fetch
```

#### Prune remotes that no longer exist

```
git fetch -p
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
