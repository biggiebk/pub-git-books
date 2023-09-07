# Understanding Resets

Reset enables you to go back to a specific commit removing the previous commits.  There are three different types of commits with, the main difference between the commit types is what is left as a status of the working directory and the index of changes being tracked, the following tables should help you understand.

We will assume the following commit history for this exercise, with the goal of resetting to commit 2af74ca.

<img src="../../.gitbook/assets/file.excalidraw (5).svg" alt="" class="gitbook-drawing">



## Three Types of Commits

### Hard

#### Process

1. Move the files that were committed in ID 1354d91 to the index
2. Copies the files that were just moved to the index to your working directory
3. HEAD is updated in the object database and now references commit 2af74ca
4. Copies the files from commit 2af74ca to the index
5. Overwrites the working with  the contents of the index (commit 2af74ca)

#### Results

| Location                     | Files          |
| ---------------------------- | -------------- |
| Working Directory            | Commit 2af74ca |
| Index                        | Commit 2af74ca |
| Object Database HEAD Pointer | Commit 2af74ca |



### Mixed (Default)

#### Process

1. Moves the files that were committed in ID 89cc67b to the index
2. Copies the files that were just moved to the index (commit 89cc67b) to your working directory
3. HEAD is updated in the object database and now references commit 2af74ca
4. Copies the files from commit 2af74ca to the index

#### Results

| Location                     | Files          |
| ---------------------------- | -------------- |
| Working Directory            | Commit 89cc67b |
| Index                        | Commit 2af74ca |
| Object Database HEAD Pointer | Commit 2af74ca |

### Soft

#### Process

1. Moves the files that were committed in ID 1354d91 to the index
2. Copies the files that were just moved to the index (commit 89cc67b) to your working directory
3. HEAD is updated in the object database and now references commit 2af74ca

#### Results

| Location                     | Files          |
| ---------------------------- | -------------- |
| Working Directory            | Commit 89cc67b |
| Index                        | Commit 89cc67b |
| Object Database HEAD Pointer | Commit 2af74ca |
