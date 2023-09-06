# Commits

## Commands

### Commit Changes

```
git commit -m "Your brief message here"
```

### Update Last Commit Message

{% hint style="info" %}
Make sure there are no fresh updates pending. When updating the last commit message any new changes will be committed along with other changes. This only works on the last commit.
{% endhint %}

git commit --amend -m "New commit message"

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

### Reset

Used to reset to a previous commit. See [understanding resets ](../how-to/understanding-resets.md)for more details on the different types.

#### Hard

```
git reset --hard <commitID>
```

#### Mixed (Default)

```
git reset <commitID>
```

#### Soft

```
git reset --soft <commitID>
```
