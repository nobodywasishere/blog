# Maintainer: Michael Riegert <michael at eowyn net>

pkgname='blog'
pkgver=0.1.2
pkgrel=1
pkgdesc='A simple command-line blog manager for Jekyll written in Python'
arch=('any')
url=https://github.com/nobodywasishere/blog
license=('GPL3')
depends=('python' 'python-argparse' 'python-simple-term-menu' 'bat')
makedepends=('python')
source=("${pkgname}"-"${pkgver}".tar.gz::${url}/archive/${pkgver}.tar.gz)
sha256sums=('SKIP')

package() {
    cd "${srcdir}"/"${pkgname}"-"${pkgver}"
    install -Dm755 blog "${pkgdir}"/usr/bin/blog
}
