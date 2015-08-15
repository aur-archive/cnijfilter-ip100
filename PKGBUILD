# Maintainer: OS Hazard <oshazard+aur@gmail.com>

pkgname=cnijfilter-ip100
pkgver=2.90
pkgrel=2
pkgdesc="Canon IJ Printer Driver for PIXMA IP100"
arch=('i686' 'x86_64')
url="http://www.canon-europe.com/Support/Consumer_Products/products/printers/InkJet/PIXMA_iP_series/iP100.aspx"
license=('GPL2' 'LGPL2' 'custom')
depends=('cnijfilter-common')
optdepends=('libglade' 'libxml' 'libtiff3' 'libpng12')
makedepends=('rpmextract')
source=('http://files.canon-europe.com/files/soft29290/Software/ip100_RPM_Linux_Driver.tgz')
md5sums=('d4adc4cd1ebb3c636a3074aa6619f410')

package() {
  cd ${srcdir}
  rpmextract.sh cnijfilter-ip100series-${pkgver}-1.i386.rpm
  install -d ${pkgdir}/usr
  mv ${srcdir}/usr/{lib,local,share} ${pkgdir}/usr/
}
