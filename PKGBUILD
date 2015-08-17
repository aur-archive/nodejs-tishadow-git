# Author: David Bankier <david@yydigital.com> (http://www.yydigital.com)
# Maintainer: dbankier <bankierd@gmail.com>
_npmname=tishadow
_repo="git://github.com/dbankier/TiShadow.git"
pkgname=nodejs-$_npmname-git
pkgver=2.5.7_dev
pkgrel=1
pkgdesc="Quick Titanium previews across devices (last dev version)"
arch=(any)
url="http://tishadow.yydigital.com"
license=(Apache Public License v2)
depends=('nodejs')
provides=('nodejs-tishadow')
conflicts=('nodejs-tishadow')
install=nodejs-tishadow.install

package() {
  cd $srcdir
  local _npmdir="$pkgdir/usr/lib/node_modules/"
  mkdir -p "$_npmdir"
  cd "$_npmdir"
  npm install -g --ignore-scripts --prefix "$pkgdir/usr" $_repo 
}

# vim:set ts=2 sw=2 et:
