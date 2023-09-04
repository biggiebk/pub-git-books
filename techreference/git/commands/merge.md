# Merge

## Types of Merges

### Fast Forward

The simplest or most straight forward type of merge.  This merge occurs when the integration branch does not contain any changes since the feature branch was originally created.  This merge is accomplished by simply updating the the commit ID of the integration branch to match that of the most recently commit ID the feature branch.

<img src="../../.gitbook/assets/file.excalidraw (3).svg" alt="" class="gitbook-drawing">

### Commit at Merge Time (Merge Commit)

This is a more complicated merge and it occurs when the integration branch has been updated after the creation of the feature branch. When this occurs GIT will create merge the two branches (assuming no [conflicts](../how-to/merge-conflicts.md)), prompt you for a commit message, and creates a new commit.

<img src="../../.gitbook/assets/file.excalidraw (4).svg" alt="" class="gitbook-drawing">

## Commands

Abort a merge attempt (only possible if there are conflicts)

```
git merge --abort
```

Merge a (feature) branch into the current (integration) branch

```
git merge <featureBrachName>
```
