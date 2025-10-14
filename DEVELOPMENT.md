# BUILDTIME REQUIREMENTS

* a UNIX-like environment (e.g. [WSL](https://learn.microsoft.com/en-us/windows/wsl/))
* [bash](https://www.gnu.org/software/bash/) 4+
* [GNU](https://www.gnu.org/)/[BSD](https://en.wikipedia.org/wiki/Berkeley_Software_Distribution) [findutils](https://en.wikipedia.org/wiki/Find_(Unix))
* [Go](https://go.dev/)
* [Python](https://www.python.org/)
* [ShellCheck](https://www.shellcheck.net/) 0.11.0+
* [Snyk](https://snyk.io/)
* Provision additional dev tools with `./install`

## Recommended

* [ASDF](https://asdf-vm.com/) 0.18 (run `asdf reshim` after provisioning)
* [direnv](https://direnv.net/) 2

# AUDIT

```console
$ ./build audit
```

# LINT

```console
$ ./build [lint]
```
