# Maintainer: McQueen <clear3239@yahoo.com>
_pkgname=xfce-simplicity
pkgname=xfce-simplicity-edition-wallpapers
pkgver=1.0.0
pkgrel=1
pkgdesc='Collection of Simplicity Edition Wallpapers Themed for XFCE'
arch=(any)
url='https://www.pling.com/p/1307493/'
license=('CC BY-NC-ND 4.0')
source=("https://github.com/MMcQueenGNU/$pkgname/$pkgname.tar.gz")
#source=(${pkgname}::"git+https://github.com/MMcQueenGNU/$pkgname")
#https://github.com/User/repo/archive/master.tar.gz
#master can be any ref, e.g. a tag.
#source=("$pkgname-$pkgver.tar.gz::https://github.com/coder/program/archive/v$pkgver.tar.gz")
#source=("${pkgname}-${pkgver}.tar.gz::https://github.com/joaopedroaats/azeny-plank/archive/v${pkgver}.tar.gz")
#source=("${pkgname}-${pkgver}.tar.gz::https://github.com/jtsiomb/xlivebg/archive/v${pkgver}.tar.gz")
#  cd "${pkgname}-${pkgver}"
#https://aur.archlinux.org/cgit/aur.git/tree/PKGBUILD?h=xlivebg
md5sums=('skip')

package() {

	cd "$srcdir/$pkgname/$_pkgname"

	# Creating needed directories
	install -dm755 "${pkgdir}/usr/share/backgrounds/$_pkgname/"

	# Wallpapers
	local wallpaper
	for wallpaper in *; do
		install -m755 "$srcdir/$pkgname-$_pkgname/${wallpaper}" "$pkgdir/usr/share/backgrounds/$_pkgname/${wallpaper}"
	done
}
