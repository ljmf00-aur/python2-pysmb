# Maintainer: Luís Ferreira <contact@lsferreira.net>
# Contributor: Levon 'noptrix' Kayan <noptrix@nullsecurity.net>

# This file is part of BlackArch Linux ( http://blackarch.org ).
# See COPYING for license details.

pkgname='python2-pysmb'
pkgver='1.1.23'
pkgrel=1
pkgdesc='An experimental SMB/CIFS library written in Python to support file sharing between Windows and Linux machines.'
arch=('any')
url='https://miketeo.net/wp/index.php/projects/pysmb'
license=('GPL')
depends=('python2')
makedepends=('python2-setuptools')
source=("https://files.pythonhosted.org/packages/67/b9/7becc03fbc39a51451a9c4497e8df2268ccccb5ee25472a1303f2e31605a/pysmb-${pkgver}.zip")
sha1sums=('b7eb338b584758b255f9263d14b2e01cf764d628')

build(){
  cd "$srcdir/pysmb-$pkgver"

  python2 setup.py build
}

package() {
  cd "$srcdir/pysmb-$pkgver"

  python2 setup.py install --root="$pkgdir" --optimize=1
}
