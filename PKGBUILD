# Contributor: Pranay Kanwar <warl0ck@metaeye.org>

pkgname=lsrtunnel
pkgver=0.2.1
pkgrel=1
pkgdesc="lsrtunnel spoofs connections using source routed packets."
url="http://www.synacklabs.net/projects/lsrtunnel/"
depends=('libpcap' 'libdnet')
license="GPL"
arch=(i686)

source=(http://www.synacklabs.net/projects/$pkgname/$pkgname-$pkgver.tar.gz)
md5sums=('5932259c08268a9510fa9d249b903d06')

build() {
  cd $startdir/src/$pkgname-$pkgver
  ./configure --prefix=/usr
  make || return 1
  make DESTDIR=$startdir/pkg install
}
