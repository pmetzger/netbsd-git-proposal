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

## Importing Git into base?

A perpetual question that gets asked is "should git be imported into
the base sources? If so, would we need to import perl?"

A proposed spectrum of answers:

1. Import into basesrc, import perl
2. Import into basesrc, don't import perl
  1. Leave the handful of perl scripts out entirely
  2. Import those perl scripts, but point at #!/usr/pkg/bin/perl --
     they will work only if someone installs perl.
3. Leave it purely to pkgsrc

I'm not sure this is really something the working group needs to
decide as such, as it doesn't really alter any of our proposed work,
but it would be nice (I think) to mention the range of options in our
proposal. I personally favor 2(ii) (not because I mind having perl in
base, but because so many other people do.) --Perry
