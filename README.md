# PKGBUILD Collection

This is a small collection of diverse `PKGBUILD` files. They are used to build
packages that can be installed to _ArchLinux_. They are just not worth to get
published as an ArchLinux User Repository.

The goal is to have everything on your computer managed as either an package of
the OS or a plugin if it is strongly related to a specific tool or environment.
The package for the OS is the always preferred approach if possible.

## Usage

```sh
cd $(mktemp --directory)
curl --output PKGBUILD https://raw.githubusercontent.com/weilbith/pkgbuild-collection/master/<select-here>.PKGBUILD
makepkg --syncdeps --install
```

## Notes

### fasd-git

This is just an adopted version of the [community
package](https://www.archlinux.org/packages/community/any/fasd/) for
[fasd](https://github.com/clvv/fasd). It basically just exchanges the upstream
source to a fork that support the
[XDG-Base-Directory](https://specifications.freedesktop.org/basedir-spec/basedir-spec-latest.html)
standard. (see also [this issue](https://github.com/clvv/fasd/issues/128)).

### zinit-git

There is no such package for [zinit](https://github.com/zdharma/zinit) so far,
but none of the documented installation approaches of the tool are acceptable.
After having it installed, use the path `/usr/share/zsh/scripts/zinit/zinit.zsh`
to source in your `zsh` setup.
