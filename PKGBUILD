# Maintainer: Pellegrino Prevete <pellegrinoprevete@gmail.com>

pkgname=gmetadom
pkgver=0.2.6
pkgrel=1
pkgdesc="DOM level2 library for accessing XML files"
arch=('any')
url="http://gmetadom.sourceforge.net/"
license=(LGPL)
depends=()
makedepends=()
source=(
  "https://sourceforge.net/projects/$pkgname/files/$pkgname/$pkgver/$pkgname-$pkgver.tar.gz/download"
)
sha512sums=(
  'SKIP'
)

build() {
  cd "${pkgname}-${pkgver}"
  ./configure \
    --prefix=/usr \
    --enable-debug=no
  make
}

package() {
  DESTDIR="$pkgdir" \
    make \
      install
}
# SPDX-License-Identifier: AGPL-3.0
#
# Maintainer: Truocolo <truocolo@aol.com>
}

# vim: ft=sh syn=sh et
# Maintainer: Pellegrino Prevete <pellegrinoprevete@gmail.com>
