# i3 Window Info

Utility tool for the [i3](https://i3wm.org/) tiling window manager. Run
`i3-win-info` and then click on any window. The console will then print out
a bunch of information of this window. This is useful to get properties that can
be used to define exact `for_window` blocks in your `i3` configuration.
Therefore it gets also represented exactly in that format as `i3` expects it.
This looks for example like that:

```sh
$ i3-win-info
[id='39845891' title='Mozilla Firefox' class='firefox' instance='Navigator' window_role='browser' workspace='1']
```

## Installation

```sh
cd $(mktemp --directory)
curl --remote-name https://raw.githubusercontent.com/weilbith/AUR/master/i3-win-info-git/PKGBUILD
mkpkg --syncdeps --install
```
