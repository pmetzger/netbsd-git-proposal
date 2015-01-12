# Open Issues Punch List

Please feel free to add more, edit, etc.

## Should the repo use git submodules

We are currently unclear on the implications of this and the stability
of the submodules support in Git

## Should we use gitolite for access control?

What other candidates are there? Are there known issues?

## Should we first do a small repo?

The notion here is that we would first do something like "othersrc" to
shake down the configuration, then (perhaps) do "pkgsrc", then "src".

## Should we have a single repository for "src"

Currently the notion is "yes", but opinions are solicited.

## *SETTLED* We will be providing a Git-to-CVS gateway

This is intended primarily for use by old, memory limited machines
that will not otherwise be able to check out sources.

## Do we want to include more history?

The old Berkeley SCCS repository and the revisions previously removed
from src because of the (now moot) lawsuit would be at issue.
