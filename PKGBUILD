#PKGBUILD for Light-Locker-Settings
# Contributor: maexbower <max@maexbower.de>
pkgname=light-locker-settings
pkgver=1.5
pkgrel=0
pkgdesc="GUI for LightLocker Settings"
arch=('any')
url="https://launchpad.net/light-locker-settings"
license=('GPL')
depends=('python' 'python-psutil' 'light-locker' 'intltool')
source=(https://launchpad.net/light-locker-settings/$pkgver/$pkgver.$pkgrel/+download/$pkgname-$pkgver.$pkgrel.tar.bz2)

build() {
  cd "$srcdir/$pkgname-$pkgver.$pkgrel"
  ./configure
  make
}

package ()
{
  cd "$srcdir/$pkgname-$pkgver.$pkgrel"
  make DESTDIR="$pkgdir" install
}

# vim:set ts=2 sw=2 et:
md5sums=('5a5dfd00deeb63b94e24cfa03548da1c')
