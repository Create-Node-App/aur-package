# Maintainer: Ulises Jeremias <ulisescf.24@gmail.com>
pkgname=create-awesome-node-app
pkgver=0.16.1
pkgrel=1
pkgdesc="Composable scaffolding CLI — one command, any Node.js stack"
arch=('any')
url="https://create-awesome-node-app.vercel.app"
license=('MIT')
depends=('nodejs>=24' 'npm')
source=("https://registry.npmjs.org/$pkgname/-/$pkgname-$pkgver.tgz")
sha256sums=('ce693c9fd8a97dddf19c05c299ad1428ba802e7103582c8856e219c9e4d9216d')

package() {
  npm install -g --prefix "$pkgdir/usr" "$srcdir/$pkgname-$pkgver.tgz"
  find "$pkgdir" -type l -xtype l -delete 2>/dev/null || true
}
