# Maintainer: anekos <anekos@snca.net>
pkgname=smart-hddtemp-daemon
pkgver=1.0.0
pkgrel=5
pkgdesc="Automatically watch all devices"
url="http://snca.net/"
arch=('i686' 'x86_64')
license=('BSD')
depends=('bash')
optdepends=()
makedepends=()
conflicts=()
replaces=()
backup=()

source=('smart-hddtemp-daemon' 'smart-hddtemp-daemon.service')
md5sums=('dc78ef6c3c492800213b12cc49d02534' '8d836c733ae51596e67278217c76e847')

package () {
  cd $srcdir

  install -d -m755 ${pkgdir}/usr/bin
  cp smart-hddtemp-daemon ${pkgdir}/usr/bin/

  install -Dm644 "smart-hddtemp-daemon.service" "$pkgdir/lib/systemd/system/smart-hddtemp-daemon.service"
}

# vim:set ts=2 sw=2 et:
