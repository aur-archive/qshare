 
# Contributor: said

pkgname=qshare
pkgver=2.1.5
pkgrel=2
pkgdesc="A FTP server with a service discovery feature that makes qShare clients aware of other clients running on the same network."
arch=('i686' 'x86_64')
url="http://www.qt-apps.org/content/show.php/qShare?content=116612"
license=('GPL3')
depends=('qt4')
source=(http://www.zuzuf.net/qshare/files/qshare-$pkgver-src.tar.bz2)
md5sums=('efafb1957a1deff1f3774de475629655')

build(){
cd $srcdir/$pkgname-$pkgver
cmake ./
make clean && make
}

package(){
cd $srcdir/$pkgname-$pkgver
make DESTDIR="${pkgdir}" install
}
