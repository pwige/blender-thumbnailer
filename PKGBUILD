pkgname=blender-thumbnailer
pkgver=1.0.0
pkgrel=1
pkgdesc='A thumbnailer for Blender project files (.blend)'
arch=('x86_64')
url="https://github.com/pwige/blender-thumbnailer"
license=('MIT')
depends=('blender')
makedepends=('git')
source=("${pkgname}::git+${url}.git#tag=${pkgver}")
b2sums=('SKIP')

package() {
	cd "$pkgname"
	mkdir -p ${pkgdir}/usr/share/thumbnailers
	cp src/*.thumbnailer ${pkgdir}/usr/share/thumbnailers/
}
