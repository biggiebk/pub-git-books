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

Used to reset to a previous commit. See [understanding resets ](../how-to/undoing-commits-reset.md)for more details on the different types.

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

### Revert

Similar to reset, however only has one mode and instead of deleting commits this one undoes the changes and then makes a new commit.

```
git revert <commitID>
```

### Specific Commit

{% hint style="info" %}
Will put the repo into headless state
{% endhint %}

```
git checkout <commitID>
```
