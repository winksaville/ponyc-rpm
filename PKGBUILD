pkgname=ponyc-rpm
pkgver=0.20.0_4003.0b2a2d2
mypkgver=("${pkgver//_/-}")
pkgrel=1
pkgdesc="ponyc installed via .rpm pkgs as ponyc is incompatible with LLVM5"
arch=('x86_64')
url="http://www.ponylang.org/"
license=('BSD')
#depends=('')
makedepends=('rpmextract')
source=("https://dl.bintray.com/pony-language/ponyc-rpm/ponyc-$mypkgver.x86_64.rpm")
md5sums=('dd4433d3f7188accc73ff1d3eabfcf20')


build() {
  cd "$srcdir"
  rpmextract.sh ../ponyc-$mypkgver.x86_64.rpm
}
package() {
  mv $srcdir/usr $pkgdir/ #/usr is the only top-level dir in the package
}
