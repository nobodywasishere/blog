# Maintainer: Michael Riegert <michael at eowyn net>

pkgname='blog'
pkgver=0.1.1
pkgrel=1
pkgdesc='A simple command-line blog manager for Jekyll written in Python'
arch=('any')
url=https://github.com/nobodywasishere/blog
license=('GPL3')
depends=('python' 'python-argparse')
makedepends=('python')
source=("${pkgname}"-"${pkgver}".tar.gz::${url}/archive/${pkgver}.tar.gz)
sha256sums=('f51a77677b90106e5fbc9c6230f46134bdad380e73b84d272550d730be9c4dd7')

package() {
    cd "${srcdir}"/"${pkgname}"-"${pkgver}"
    install -Dm755 blog "${pkgdir}"/usr/bin/blog
}
