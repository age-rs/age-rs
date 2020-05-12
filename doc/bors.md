# Buildbot commands (Bors)

Syntax | Description
-------|------------
bors r+ | Run the test suite and push to master if it passes. Short for "reviewed: looks good."
bors merge | Equivalent to `bors r+`.
bors r=[list] | Same as r+, but the "reviewer" in the commit log will be recorded as the user(s) given as the argument.
bors merge=[list] | Equivalent to `bors r=[list]`
bors r- | Cancel an r+, r=, merge, or merge=
bors merge- | Equivalent to `bors r-`
bors try | Run the test suite without pushing to master.
bors try- | Cancel a try
bors delegate+ <br> bors d+ | Allow the pull request author to r+ their changes.
bors delegate=[list] <br> bors d=[list] | Allow the listed users to r+ this pull request's changes.
bors ping | Check if bors is up. If it is, it will comment with _pong_.
bors retry | Run the previous command a second time.
bors p=[priority] | Set the priority of the current pull request. Pull requests with different priority are never batched together. The pull request with the bigger priority number goes first.
bors r+ p=[priority] | Set the priority, run the test suite, and push to master (shorthand for doing p= and r+ one after the other).
bors merge p=[priority] | Equivalent to `bors r+ p=[priority]`
