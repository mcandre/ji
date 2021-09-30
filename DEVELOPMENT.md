# BUILDTIME REQUIREMENTS

* [accio](https://github.com/mcandre/accio)
* [bashate](https://pypi.python.org/pypi/bashate/0.5.1)
* [checkbashisms](https://sourceforge.net/projects/checkbaskisms/)
* [coreutils](https://www.gnu.org/software/coreutils/)
* [ShellCheck](https://hackage.haskell.org/package/ShellCheck)
* [vast](http://github.com/mcandre/vast)

## Recommended

* [Debian](https://www.debian.org/)

# BUILD: LINT + TEST

```console
$ vast
```

# LINT

```console
$ vast ilint
```

# TEST

Warning: Test may prompt for a system reboot.

```console
$ vast itest
```
