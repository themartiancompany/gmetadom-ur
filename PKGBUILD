# SPDX-License-Identifier: AGPL-3.0
#
# Maintainer: Pellegrino Prevete <pellegrinoprevete@gmail.com>
# Maintainer: Truocolo <truocolo@aol.com>

pkgname=gmetadom
pkgver=0.2.6
pkgrel=1
pkgdesc="DOM level2 library for accessing XML files"
arch=(
  'any'
)
url="http://${pkgname}.sourceforge.net"
license=(
  LGPL
)
depends=(
  gdome2
)
makedepends=()
_sourceforge="https://sourceforge.net/projects"
_url="${_sourceforge}/${pkgname}/files/${pkgname}/${pkgver}/${pkgname}-${pkgver}.tar.gz/download"
source=(
  "${pkgname}-${pkgver}.tar.gz::${_url}"
)
sha512sums=(
  '69521b8d667d832259687d34c8855ece51fbcbffe3b54a8d588cad402cb45e8e30259b0627dd0badc4aa7efcf39f8ceb3c62eb76916ca1104481f65ddc31c6bf'
)

build() {
  cd \
    "${pkgname}-${pkgver}"
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

# vim: ft=sh syn=sh et
