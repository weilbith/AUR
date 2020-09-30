# shellcheck disable=SC2034

_pkgname=fasd
pkgname=${_pkgname}-git
pkgver=1
pkgrel=1
pkgdesc='Command-line productivity booster, offers quick access to files and directories'
arch=('any')
url='https://github.com/whjvenyl/fasd'
license=('MIT')
makedepends=('git')
source=('git+https://github.com/whjvenyl/fasd.git')
sha256sums=('SKIP')
provides=('fasd')
conflicts=('fasd')

pkgver() {
  cd "$_pkgname"
  printf "r%s.%s" "$(git rev-list --count HEAD)" "$(git rev-parse --short HEAD)"
}

package() {
  cd "$_pkgname"
  make DESTDIR="$pkgdir" PREFIX=/usr install
  install -D --mode=644 LICENSE "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
  install -D --mode=644 README.md "$pkgdir/usr/share/doc/$pkgname/README.md"
}

# vim: tabstop=2 shiftwidth=2 filetype=PKGBUILD
