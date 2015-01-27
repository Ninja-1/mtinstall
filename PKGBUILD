pkgname=mtinstall
pkgver=1.5
pkgrel=1
pkgdesc="Bridge Linux install script"
url="http://millertechnologies.net/"
arch=('any')
license=()
source=(mtinstall.tar.xz)
md5sums=('c67a97e7f40b7245e137fe2b5952c215')

build() {
   cd $srcdir
   msg2 "Extracting source..."
   tar -xf mtinstall.tar.xz
}

package() {
   cd "$srcdir"

   msg2 "Copying files..."
   mkdir -p $pkgdir/usr/bin
   mkdir -p $pkgdir/etc/skel/Desktop
   mkdir -p $pkgdir/usr/lib/mtinstall
   cp bin/mtinstall "$pkgdir/usr/bin/mtinstall"
   cp bin/installer.desktop "$pkgdir/etc/skel/Desktop"
   cp -a locales "$pkgdir/usr/lib/mtinstall"
}
