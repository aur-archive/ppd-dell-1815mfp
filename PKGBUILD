# Maintainer: Martin Wimpress <code@flexion.org>

pkgname=ppd-dell-1815mfp
pkgver=1.21.A03
pkgrel=2
pkgdesc="Printer only driver for the Dell MFP Laser Printer 1815dn"
arch=(any)
url="http://www.dell.com/support/drivers/uk/en/ukbsdt1/DriverDetails/DriverFileFormats?c=uk&l=en&s=bsd&cs=ukbsdt1&DriverId=R143817"
license=('custom')
depends=('cups')
optdepends=()
source=("http://downloads.dell.com/printer/Driver_ONLY_Linux.tar.gz")
md5sums=('33ca2067135e7ece09bb23db5f84b202')

package() {
  install -d "${pkgdir}/usr/share/cups/model/Dell"
  install "${srcdir}/cdroot/Linux/noarch/at_opt/share/ppd/mfp1815ps.ppd" "${pkgdir}/usr/share/cups/model/Dell"
}
