# Merge Conflicts

How to deal with merge conflicts

Example of conflict message when merging

```
git merge testBranch1
Auto-merging test.md
CONFLICT (content): Merge conflict in test.md
Automatic merge failed; fix conflicts and then commit the result.
```

Run git status for details

```
git status
On branch master
You have unmerged paths.
  (fix conflicts and run "git commit")
  (use "git merge --abort" to abort the merge)

Unmerged paths:
  (use "git add <file>..." to mark resolution)
        both modified:   test.md

no changes added to commit (use "git add" and/or "git commit -a")
```

Edit the file to resolve conflict.  Here is the example of what a conflicted file looks like.

```
Orig file line one
<<<<<<< HEAD
This is the second line from the intigration branch
=======
This is a second line from feature branch
>>>>>>> testBranch1
```

* &#x20;<<<<<<< - Denotes the start of the conflict
* HEAD  - indicates the next line(s) are in the integration branch
* &#x20;\=======  - End of the integration branch line(s) and start of the feature branch
* &#x20;\>>>>>>>  - end of the feature branch line(s)
* testBranch1 - the name of the feature branch

Finally add/stage the file and commit

```
git add test.md
git commit -m "Resolve merge conflict with testBranch1"
```
