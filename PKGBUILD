# Maintainer: Alexander Rødseth <rodseth@gmail.com>
pkgname=vanilla
pkgver=2.0.18.2
pkgrel=2
pkgdesc='Light weight forum written in PHP'
arch=('any')
url='http://vanillaforums.org/'
license=('GPL')
depends=('php' 'php-gd')
optdepends=("apache: Web server to run $pkgname"
            "cherokee: Lightweight Web server to run $pkgname"
            'mysql: Database server')
options=(emptydirs)
install=$pkgname.install
source=("http://vanillaforums.org/get/$pkgname-core.zip")
sha256sums=('3113a1238b21d61be4a1b93fb79c7d950a78bbdad7eda099d55ce65cb79a30bf')

package() {
  cd "$srcdir"

  install -d "$pkgdir/srv/http"
  cp -r "$pkgname" "$pkgdir/srv/http"
}

# vim:set ts=2 sw=2 et:
