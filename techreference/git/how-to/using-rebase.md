# Using Rebase

A rebase changes the original commit that a branch was created from to the most recent commit of the originating branch.  It replays the additional commits against the new branch and could lead to merge conflicts. Doing so will help flatten the branches and make merging back to the original branch less complicated. In this example we will use the Master branch as the originating branch and a feature branch as the working branch we want to rebase.

<img src="../../.gitbook/assets/file.excalidraw (7).svg" alt="" class="gitbook-drawing">

{% hint style="info" %}
Note the Commit ID's changed on the feature branch.
{% endhint %}

All you have to do is run the following command from the Feature branch and will automatically update to the Masters most recent commit ID.

```
git rebase
```
