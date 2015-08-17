# Maintainer: Robin Baumgartner <robin@baumgartners.ch>
pkgname=trytond-country
_pkgname=trytond_country
pkgver=3.4.1
_pkgdir=3.4
pkgrel=1
pkgdesc="The country module of the Tryton application platform"
arch=('any')
url='http://www.tryton.org/'
license=('GPL3')
groups=('trytond-modules')
depends=('trytond>=3.4')
makedepends=('python2-distribute')
source=("http://downloads.tryton.org/$_pkgdir/$_pkgname-$pkgver.tar.gz")
md5sums=("6628ee67c310284eef211fe3a9fc661c")

build() {
  cd $srcdir/$_pkgname-$pkgver
  python2 setup.py build
}

package() {
  cd $srcdir/$_pkgname-$pkgver
  python2 setup.py install --root=$pkgdir
}