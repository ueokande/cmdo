cmdo
====

A package manager and bundler for commands on terminal.

The basic concept is inspired by modern package manager in many language, such
as gem, go-get, and npm.  Cmdo is written in POSIX sh.  It works in any
Unix-like operation systems.

Installation
------------

```sh
curl -sSL https://ueokande.github.io/cmdo/install | sh -s
```

Usage
-----

You can install a repository via github.com as following:

```sh
cmdo install github.com/ueokande/tegrep
```

All commands of cmdo is the following:

- `install` - installs a package from remote repository
- `list` - displays installed packages
- `update` - update a package
- `remove` - removes a package from local disk
- `fetch` - downloads a package into local disk, but not installs a package

Requirements for a package
--------------------------

Cmdo installs a package fetches by using git-clone into local disk, and copy
files in the repository to `$HOME/.cmdo`.  The copied files are files in `bin`
on the root of repository, and executable files on the root.

To make a package worked with cmdo, put executable files on the root of the
repository, or `bin` directory in the root directory.

Licence
-------

MIT
