# Working with Bisect

Bisect allows for a binary search. Meaning that you can pick two commits one that you know is good (known to be good) and one that is bad (You know it has the problem). Git will then pick the middle commit and update your working directory to match that commit. Once you review that commit you can say whether that commit is bad (go further down) or good (move up).  And so on...

We will work off of a repo with the following commit history.

<img src="../../.gitbook/assets/file.excalidraw (6).svg" alt="" class="gitbook-drawing">

## Start the session

We need to start the session and choose the good bad. For our purpose we will assume e5c03e7 is bad and 30d8881 is good.

```
git bisect start
git bisect bad e5c03e7
git bisect good 30d8881
```

Git will then look at the list of commits between e5c03e7 and 30d8881 pick the middle most commit.  In this case our working directory will be updated to match commit 43ece6c.

## Moving up or down the commit history

### Bad (Down)

If you find that the current commit is still bad you can simply run.

```
git bisect bad
```

and it will move to the middle commit between 43ece6c and 30d8881.

### Good (Up)

If you determine that this commit is good and you want to up to a commit between e5c03e7 and 43ece6c you would run the following.

```
git bisect good
```

## Ending Your Session

You need to run the following to end your session.

```
git bisect reset
```

### Am I Still in My Bisect Session?

If you are unsure if your session is still valid you can run a status.

```
git status
```
