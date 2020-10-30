# Fasd

This is just an adopted version of the [community
package](https://www.archlinux.org/packages/community/any/fasd/) for
[fasd](https://github.com/clvv/fasd). It basically just exchanges the upstream
source to a fork that support the
[XDG-Base-Directory](https://specifications.freedesktop.org/basedir-spec/basedir-spec-latest.html)
standard. (see also [this issue](https://github.com/clvv/fasd/issues/128)).

## Installation

```sh
cd $(mktemp --directory)
curl --remote-name https://raw.githubusercontent.com/weilbith/pkgbuild-collection/master/fasd-git/PKGBUILD
mkpkg --syncdeps --install
```
