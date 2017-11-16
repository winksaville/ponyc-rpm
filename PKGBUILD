# Maintainer: Wink Saville <wink@saville.com>
pkgname=ponyc-rpm
pkgver=0.20.0_4003.0b2a2d2
_pkgver=("${pkgver//_/-}")
pkgrel=1
pkgdesc="ponyc installed via .rpm pkgs as ponyc is incompatible with LLVM5"
arch=('x86_64')
url="http://www.ponylang.org/"
license=('BSD')
depends=('zlib' 'ncurses5-compat-libs')
source=("https://dl.bintray.com/pony-language/ponyc-rpm/ponyc-${pkgver//_/-}.$CARCH.rpm")
md5sums=('dd4433d3f7188accc73ff1d3eabfcf20')

package() {
  cp -a $srcdir/usr $pkgdir/
  install -Dm644 $srcdir/../LICENSE "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
}
