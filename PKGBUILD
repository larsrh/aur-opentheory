# Maintainer: Ramana Kumar <at gmail dot com>
pkgname=opentheory
pkgver=1.3r20160204
pkgrel=1
pkgdesc="a tool for processing higher-order logic theory packages"
arch=('i686' 'x86_64')
url="http://www.gilith.com/software/opentheory"
license=('MIT')
groups=()
depends=()
makedepends=(mlton)
source=($pkgname-$pkgver.tar.gz::$url/$pkgname.tar.gz)
md5sums=('e576e0a023c360dd3263ac332d9c3562')

build() {
  cd "$srcdir/$pkgname"
  make mlton
}

package() {
  mkdir -p "$pkgdir/usr/bin"
  cp -p "$srcdir/$pkgname/bin/mlton/$pkgname" "$pkgdir/usr/bin/$pkgname"
}

# vim:set ts=2 sw=2 et:
