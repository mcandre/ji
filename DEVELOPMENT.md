# BUILDTIME REQUIREMENTS

* [bash](https://www.gnu.org/software/bash/)
* [GNU](https://www.gnu.org/)/[BSD](https://en.wikipedia.org/wiki/Berkeley_Software_Distribution) [findutils](https://en.wikipedia.org/wiki/Find_(Unix))
* [POSIX](https://pubs.opengroup.org/onlinepubs/9799919799/) compatible [make](https://en.wikipedia.org/wiki/Make_(software))
* [ShellCheck](https://www.shellcheck.net/) 0.10.0+
* [Go](https://go.dev/) 1.24.6+
* [Python](https://www.python.org/) 3.13.7+
* [Rust](https://www.rust-lang.org/) 1.87.0+
* [Snyk](https://snyk.io/)
* Provision additional dev tools with `make -f install.mk [-j 4]`

## Recommended

* [ASDF](https://asdf-vm.com/) 0.10 (run `asdf reshim` after provisioning)
* [direnv](https://direnv.net/) 2
* [GNU](https://www.gnu.org/)/[BSD](https://en.wikipedia.org/wiki/Berkeley_Software_Distribution) [make](https://en.wikipedia.org/wiki/Make_(software))
* [zsh](https://www.zsh.org/)

# AUDIT

```console
$ make audit
```

# LINT

```console
$ make [lint]
```
