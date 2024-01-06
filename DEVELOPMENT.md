# BUILDTIME REQUIREMENTS

* a UNIX environment with [coreutils](https://www.gnu.org/software/coreutils/) / [base](http://ftp.freebsd.org/pub/FreeBSD/releases/) / [macOS](https://www.apple.com/macos) / [WSL](https://learn.microsoft.com/en-us/windows/wsl/install) / etc.
* a POSIX compliant [make](https://pubs.opengroup.org/onlinepubs/9699919799/utilities/make.html) implementation (e.g. GNU make, BSD make, etc.)
* GNU compatible [findutils](https://www.gnu.org/software/findutils/)
* [GNU grep](https://www.gnu.org/software/grep/)
* [ShellCheck](https://hackage.haskell.org/package/ShellCheck)
* [Go](https://go.dev/) 1.21.5+
* [Python](https://www.python.org/) 3.12.1+
* [Rust](https://www.rust-lang.org/) 1.75.0+
* Provision additional dev tools with `make -f install.mk`

## Recommended

* [macOS](https://www.apple.com/macos), or [Debian](https://www.debian.org/) / [Ubuntu](https://ubuntu.com/)
* [ASDF](https://asdf-vm.com/) 0.10 (run `asdf reshim` after provisioning)
* [direnv](https://direnv.net/) 2

# AUDIT

```console
$ make audit
```

# LINT

```console
$ make [lint]
```
