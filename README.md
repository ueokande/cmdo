cmdo
====

Command package manager and bundler.  The basic concept is inspired by modern
package manager in many language, such as gem, go-get, and npm.

Installation
------------

```sh
\curl -sSL https://raw.githubusercontent.com/ueokande/cmdo/blob/master/scripts/install | bash -s
```

Usage
-----

You can install a repository via github.com as following:

```sh
cmdo install github.com/ueokande/tegrep
```

All commands

- `install` - installs a package from remote repository
- `list` - displays installed packages
- `update` - update a package
- `remove` - removes a package from local disk
- `fetch` - downloads a package into local disk, but not installs a package
