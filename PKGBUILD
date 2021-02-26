# Maintainer: Michael Riegert <michael at eowyn net>

pkgname='blog-git'
pkgver=210226
pkgrel=1
pkgdesc='A simple command-line blog manager for Jekyll written in Python'
arch=('any')
url=https://github.com/nobodywasishere/blog
license=('GPL3')
depends=('python' 'python-argparse' 'python-simple-term-menu' 'bat')
makedepends=('python')
source=(${pkgname}::git+${url})
sha256sums=('SKIP')

pkgver() {
	date +%y%m%d
}

package() {
    cd "${srcdir}/${pkgname}"
    install -Dm755 blog "${pkgdir}"/usr/bin/blog
}
