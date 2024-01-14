# Relative Commit Referencing

## Previous Commits (\~n)

You can use the operator \~n, where n is the number from the commits from the referenced commit. You can reference the initial commit using either HEAD or the CommitID. The following commit history shows examples of how each commit could be referenced.

<img src="../../.gitbook/assets/file.excalidraw (1) (1).svg" alt="" class="gitbook-drawing">

### Alias

Using a \~ minus the number is an alias for \~1.  Given the above a \~ by itself is a reference to commit ID 6f09339.

## Traversing Merge Commits (^n)

[Merge commits](../the-basics/merge.md#commit-at-merge-time-merge-commit) have two parents. You can reference the individual parent by using the operator ^n, where n is either 1 for the first parent or 2 for the second parent. (HEAD^1 and HEAD^2).&#x20;

<img src="../../.gitbook/assets/file.excalidraw (1) (1) (1).svg" alt="" class="gitbook-drawing">

## Combining Both Operators (^n\~n)

Finally you can combine the two operators for more complex referencing.

<img src="../../.gitbook/assets/file.excalidraw (2) (1).svg" alt="" class="gitbook-drawing">
