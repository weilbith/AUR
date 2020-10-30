# Zinit

There is no package for [zinit](https://github.com/zdharma/zinit) so far and
none of the documented installation approaches is acceptable.

After having it installed, use the path `/usr/share/zsh/scripts/zinit/zinit.zsh`
to source in your `zsh` setup.

## Installation

```sh
cd $(mktemp --directory)
curl --remote-name https://raw.githubusercontent.com/weilbith/AUR/master/zinit-git/PKGBUILD
mkpkg --syncdeps --install
```
