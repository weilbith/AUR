# TMux Thumbs

There is no package for [tmux-thumbs](https://github.com/fcsonline/tmux-thumbs)
so far and none of the documented installation approaches is acceptable.

After having it installed, use the following line in your `tmux` configuration:
`run-shell /usr/share/tmux/plugins/tmux-thumbs/tmux-thumbs.tmux`.

## Installation

```sh
cd $(mktemp --directory)
curl --remote-name https://raw.githubusercontent.com/weilbith/pkgbuild-collection/master/tmux-thumbs-git/PKGBUILD
mkpkg --syncdeps --install
```
