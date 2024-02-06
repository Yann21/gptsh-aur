pkgname=gptsh
pkgver=0.0.1
_pkgname=gptsh
pkgrel=1
pkgdesc="A command-line interface for GPT"
arch=('any')
url="https://npmjs.com/package/gptsh"
license=('MIT')
depends=('nodejs' 'npm')
makedepends=('npm')


package() {
  npm install -g --prefix "${pkgdir}/usr" "${srcdir}/${_pkgname}-${pkgver}.tgz"

}

