# remove_DS_Store_git_hook

## Usage
Move or symlink to (git repo)/.git/hooks/precommit

This hook does not just prevent a commit adding .DS_Store files, it *actively removes* any files called .DS_Store that have been git-add-ed from the repository index (not from the disk).

Modify the FORBIDDEN variable in the hook to exclude a different filename.

If you want to exclude filenames that match a pattern, this is a good overview of patterns in bash: https://stackoverflow.com/a/37038262
