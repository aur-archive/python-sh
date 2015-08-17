# Maintainer : Daniel Wallace <danielwallace at gtmanfred dot com>

_pkgname=sh
pkgname=python-$_pkgname
pkgver=1.07
pkgrel=1
pkgdesc="A full-fledged subprocess interface for Python that allows you to call any program as if it were a function"
arch=('any')
url=('http://amoffat.github.com/sh/index.html')
license=("MIT")
depends=('python')
makedepends=('python-distribute')
source=(
  "http://pypi.python.org/packages/source/s/sh/$_pkgname-$pkgver.tar.gz"
)

md5sums=('68edad68bd108df713f1424bc65468e9')

build() {
  cd $srcdir/$_pkgname-$pkgver
  python setup.py build
}


package() {
  cd $srcdir/$_pkgname-$pkgver
  python setup.py install --root=$pkgdir
}
