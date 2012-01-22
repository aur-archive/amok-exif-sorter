# Author: Andreas Krist <group@amok.am>
# Contributor: Xi0N <grayfox.i0n@gmail.com>

pkgname=amok-exif-sorter
pkgver=2.56
pkgrel=1
pkgdesc="AmoK Exif Sorter is the easy but powerful solution for renaming your photos using EXIF data"
arch=(i686 x86_64)
url="http://www.amok.am/en/freeware/amok_exif_sorter/" 
license=(FREEWARE)
depends=('java-runtime')

_source_arch="32Bit"
[ "$CARCH" = "x86_64" ] && _source_arch="64Bit"

md5sums=('144f34d48eedf82e93b42426a5c01e50'
	'75dfb58bc9a737255e313de70b8326bf'
	'cbae880ef6fce7d00f1a928679c3d252')
[ "$CARCH" = "x86_64" ] && md5sums[0]='084587577652e01835fcc306f3a55773'

source=("http://www.amok.am/files/releases/AmoK_Exif_Sorter_v${pkgver}_(Linux_${_source_arch}).tar.bz2"
	"amok-exif-sorter.desktop"
	"amok-exif-sorter.png")

build() {
	install -D amok-exif-sorter.desktop $pkgdir/usr/share/applications/amok-exif-sorter.desktop
	mkdir -p $pkgdir/opt/AmokExifSorter/
	cp -Lrp * $pkgdir/opt/AmokExifSorter/
}
