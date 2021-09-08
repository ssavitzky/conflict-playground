# Git merge/rebase playground

This repo is meant to be used for playing with `git merge`, `git rebase`,
conflict resolution, merge tools, and so on.

There is a file called `sample.txt` that can be used to set up different
scenarios, each of which is contained in a separate branch. The branches are:

**main**: documentation.  This branch also contains `sample.txt` in its
original form.

**us**, **them**: each of these modifies the sample in different, conflicting
ways. The intended usage is `git checkout us; git merge them`.

**delete**: deletes `sample.txt`, for setting up delete/modify conflicts when
merged with either `us` or `them`.

**move**: renames `sample.txt` to `moved.txt`.  This creates a somewhat more
complicated delete/modify conflict.

**move-modify** both renames `sample.txt` and modifies it.  Resolving this
may involve merging the original and modified versions of the file.

