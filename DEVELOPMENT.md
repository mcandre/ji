# BUILDTIME REQUIREMENTS

* a UNIX environment with [coreutils](https://www.gnu.org/software/coreutils/) / [base](http://ftp.freebsd.org/pub/FreeBSD/releases/) / [macOS](https://www.apple.com/macos) / [WSL](https://learn.microsoft.com/en-us/windows/wsl/install) / etc.
* GNU compatible [findutils](https://www.gnu.org/software/findutils/)
* [GNU grep](https://www.gnu.org/software/grep/)
* [ShellCheck](https://hackage.haskell.org/package/ShellCheck)
* [vast](http://github.com/mcandre/vast) 0.0.1
* [Go](https://go.dev/) 1.20.2+ with `go install github.com/mcandre/accio/cmd/accio@v0.0.4` and `accio -install`
* [Python](https://www.python.org/) 3.11.2+ with `pip[3] install --upgrade pip setuptools` and `pip[3] install -r requirements-dev.txt`

## Recommended

* [macOS](https://www.apple.com/macos), or [Debian](https://www.debian.org/) / [Ubuntu](https://ubuntu.com/)
* [ASDF](https://asdf-vm.com/) 0.10
* [direnv](https://direnv.net/) 2

# AUDIT

```console
$ vast v-audit
```

# BUILD: LINT + TEST

```console
$ vast [v-build]
```

# LINT

```console
$ vast v-lint
```

# TEST

Warning: Test may prompt for a system reboot.

```console
$ vast v-test
```
