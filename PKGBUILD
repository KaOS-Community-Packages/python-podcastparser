
_pkgname=podcastparser
pkgname=python-$_pkgname
pkgver=0.6.4
pkgrel=1
pkgdesc="podcast parser for gpodder"
arch=('x86_64')
url="http://gpodder.org/podcastparser/"
license=('ISC')
depends=('python3')
source=(https://github.com/gpodder/podcastparser/archive/$pkgver.tar.gz)
md5sums=('93eb67ce21165bf3f79a4a8b40e021fd')

package() {
  cd $srcdir/${_pkgname}-${pkgver}
  python3 setup.py install --root=$pkgdir --optimize=1
  install -Dm644 LICENSE "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
}
