Setting up a blank repo
=======================

To create an empty repo to push into:

```
$ git init --bare sybase-logs.git
```

Then in the working copy:

```
$ git remote add origin sysdevlx1.london.daiwa.global:git/sybase-logs.git
```

or:

```
$ git remote set-url origin sysdevlx1.london.daiwa.global:git/sybase-logs.git
```

If you need to re-write the branch.master section:

```
$ git config --remove-section branch.master
```

To re-add:

```
$ git config branch.master.remote origin
$ git config branch.master.merge refs/heads/master
```
