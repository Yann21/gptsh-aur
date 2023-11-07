pkgname=gptsh
pkgver=0.0.1
pkgrel=1
pkgdesc="A command-line interface for GPT"
arch=('any')
url="https://npmjs.com/package/gptsh"
license=('MIT')
depends=('nodejs' 'npm')
makedepends=('npm')

package() {
  # Install the package locally
  npm install gptsh

  # Move the local installation to the global directory
  mkdir -p "$pkgdir/usr/lib/node_modules/"
  cp -r node_modules/gptsh "$pkgdir/usr/lib/node_modules/"
  
  # Symlink the binary to the system's bin directory so it's available in PATH
  mkdir -p "$pkgdir/usr/bin/"
  ln -s /usr/lib/node_modules/gptsh/src/index.js "$pkgdir/usr/bin/gptsh"
}

