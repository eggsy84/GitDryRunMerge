GitDryRunMerge
==============

This git hook should be executed during the 'post commit' (hence the name) phase of a git lifecycle.

The git hook is designed to perform a dummy merge of the current branch with any target branch. It then reports whether the merge
will result in conflicts or whether the merge should be fine. If there are possible conflicts the hook will report which files might be
a problem.

Upon making a commit, the hook will execute asking the developer if they wish to try a dummy merge with
another branch. The developer then enters a branch name and the hook will try a dummy merge with the given branch.

If the developer does not wish to perform a dry-run merge simply press <return> without entering a branch or press escape.

An example of its usage with a short description can be found on http://eggsylife.co.uk/2013/10/05/git-post-commit-dummy-merge/

