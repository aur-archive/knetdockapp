# Contributor: Sergej Pupykin <pupykin.s+arch@gmail.com>
# Contributor : Todd Maynard <arch@toddmaynard.com>

pkgname=knetdockapp
pkgver=0.82.3
pkgrel=1
pkgdesc="KDE systray app that monitors the activity of network interfaces and the link status."
arch=('i686' 'x86_64')
url="http://www.kde-apps.org/content/show.php?content=29398"
license=('GPL')
depends=('kdelibs3')
source=(http://www.kde-apps.org/CONTENT/content-files/29398-$pkgname-$pkgver.tar.bz2)
md5sums=('701db6bf6ad966609162b598dd09aaaf')

build() {
  cd $srcdir/$pkgname-$pkgver
#  ./autogen.sh
  ./configure --prefix=/opt/kde --without-arts
  make || return 1
  make DESTDIR=$pkgdir install
}
