# Maintainer: McQueen <clear3239@yahoo.com>
_pkgname=xfce-simplicity
pkgname=xfce-simplicity-edition-wallpapers
pkgver=1.0.0
pkgrel=1
pkgdesc='Collection of Simplicity Edition Wallpapers Themed for XFCE'
arch=(any)
url='https://www.pling.com/p/1307493/'
license=('CC BY-NC-ND 4.0')
source=("https://github.com/MMcQueenGNU/$pkgname/releases/download/$pkgver/$pkgname-$pkgver.tar.xz")
md5sums=('skip')

package() {

	cd "$srcdir/$pkgname-$pkgver/"

	# Creating needed directories
	install -dm755 "${pkgdir}/usr/share/backgrounds/$_pkgname/"

	# Wallpapers
	local wallpaper
	for wallpaper in *; do
		install -m755 "$srcdir/$pkgname-$pkgver/${wallpaper}" "$pkgdir/usr/share/backgrounds/_pkgname/${wallpaper}"
	done
}
