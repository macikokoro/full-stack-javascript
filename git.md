# Git

To install git make sure to have homebrew installed. Run `brew install git` in the Terminal and you are set.

## Useful Git Commands

`git ls-remote` \| list remote branches

`git config --global --edit` \| edit conf file

`git commit --amend --reset-author` \| fix indentity used.

## If you ever run in trouble like I do the following will help you out.

`rm -rf directory-name` \| Removes a directory with contents

`rm -rf .git` \| Removes git from directory. Make sure that you absolutely need to this, it will delete everything from branches to commits.

`git reset --hard HEAD` \| This will bring you back to your last commit and will ignore any new changes made after.

`git branch -d branch-name'` \| Deletes a branch.

