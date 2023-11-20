# Using Aliases

Not so much a how to as a these are the aliases that I commonly setup for myself at the global level.

## Create Alias Commands

```bash
# Log with online and graph
git config --global alias.l  "log --graph --oneline"

# Log with graph and abbrev-commit
git config --global alias.lv  "log --graph --abbrev-commit"

# Commit with message option preset
git config --global alias.co "commit -m"

# Basic push
git config --global alias.p "push"

# Forch push
git config --global alias.pf "push -f"

# Clone
git config --global alias.cl "clone"

# List all branches
git config --global alias.b "branch -a"

# Switch
git config --global alias.sw "switch"

# Switch with create flag preset
git config --global alias.swc "switch -c"

# Add command
git config --global alias.a "add"

# Full status
git config --global alias.stf "status"

# Short status with branches
git config --global alias.st "status -s -b"

# Grep with line numbers
git config --global alias.g "grep -n"

# List count configured aliases
git config --global alias.ca "config --get-regex ^alias\."

```

## From git to g

### BASH

Add this to your profile

```bash
alias g=/path/to/git
```

### Fish

This will save it to your profile

```bash
alias --save g /path/to/git
```

### PowerShell (Windows)

Add this line to your PowerShell profile

```powershell
Set-Alias -name g -value "c:\path\to\git.exe'
```
