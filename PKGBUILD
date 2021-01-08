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
sha256sums=('54cd0b6d20c5b5e67fc57e2f712e837e536d2356d644af3981a2e7a9e126f876')

package() {
    cd "${srcdir}"/"${pkgname}"-"${pkgver}"
    install -Dm755 blog "${pkgdir}"/usr/bin/blog
}
