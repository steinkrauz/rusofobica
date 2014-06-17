# Maintainer: Stein Krauz steinkrauz@yahoo.com>
pkgname=rusofobica
pkgver=1.0
pkgrel=1
pkgdesc="Decent keyboard layout for Russian"
arch=(any)
license=('GPL')
url="http://lj.rossia.org/users/lookatmoron/162974.html"
depends=('xkbdata')
source=(rusofobica-${pkgver}.tar.gz)
md5sums=('b27b9306fdeee9c52ee67c49e0665e6c')
install=rusofobica.install

package() {
  cd "${srcdir}/${pkgname}-${pkgver}"
  install -D -m644 rf ${pkgdir}/usr/share/X11/xkb/symbols/rf
  install -D -m644 evdev.patch ${pkgdir}/usr/share/rusofobica/evdev.patch
}
