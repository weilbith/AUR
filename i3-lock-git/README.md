# i3 Lock

Utility tool for the [i3](https://i3wm.org/) tiling window manager. Used to lock
your screen (e.g. with `xautolock`). It is basically just wraps the
[i3lock-color](https://github.com/Raymo111/i3lock-color) tool with some custom
configuration. The executable is named `i3-lock`.
The to use wallpaper image file path can be either provided via
the environment variable `WALLPAPER_IMAGE_FILE` or as first parameter to the
command. The chosen colors follow the Blue Planet palette.

## Installation

This package includes a dependency that is only available as AUR. This can not
be resolved by `makepkg --syncdeps` which uses per default `pacman`. Therefore
you need a AUR helper. `makepkg` uses the environment variable `PACMAN` to
define the program to resolve dependencies. Unfortunately does no helper I know
work correctly here. So does for example `yay` use different exit codes
`makepkg` don't understand. Issue to resolve that problem is still open. Anyways
I can recommend to use the AUR helper
[pikaur](https://github.com/actionless/pikaur) which does support to install
`PKGBUILD` files on the host natively. Alternatively you can install the
`i3lock-color` dependency manually before installing this package here.

```sh
cd $(mktemp --directory)
curl --remote-name https://raw.githubusercontent.com/weilbith/AUR/master/i3-lock-git/PKGBUILD
pikaru --pkgbuild --install
```
