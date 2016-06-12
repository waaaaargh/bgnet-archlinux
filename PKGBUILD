# Packager: Johannes Fürmann <johannes@weltraumpflege.org>

pkgname=bgnet
pkgver=3.0.21
pkgrel=1
pkgdesc="Beejs Guide to Network Programming"
arch=(any)
license=(Proprietary)
url=https://beej.us/guide/bgnet/
options=(docs)
depends=()
source=(
	https://beej.us/guide/bgnet/output/html/bgnet_multipage.tgz
	bgnet.sh
)

build() {
  cd $srcdir
  tar xzf bgnet_multipage.tgz
}

package() {
  mkdir -p $pkgdir/usr/share/doc/bgnet
  cp -r $srcdir/bgnet/* $pkgdir/usr/share/doc/bgnet
  mkdir -p $pkgdir/usr/bin/
  cp $srcdir/bgnet.sh $pkgdir/usr/bin/bgnet
}

sha256sums=(
	'9e4ec7becc4db05de5424b9150a339541b8b1060be8db6964f4a3bb84f94e17d'
        '5db12b3a121990d427128180ff13310231f7d88360fd3375344d628e289269b5'
)
