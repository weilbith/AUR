# i3 Goto Mark

Utility tool for the [i3](https://i3wm.org/) tiling window manager. It opens
a menu to select from all windows with a marker. Jumps to the selected window or
aborts.

Not automatically included requirements:

- `i3-msg` (assumed to be installed by `i3` itself)
- `dmenu`, `rofi` (or alternative listed as optional dependency)

## Installation

```sh
cd $(mktemp --directory)
curl --remote-name https://raw.githubusercontent.com/weilbith/AUR/master/i3-goto-mark-git/PKGBUILD
mkpkg --syncdeps --install
```

It is recommended to put a key binding into your `i3` configuration for it like
so:

```i3
bindsym $mod+g exec i3-goto-mark
```
