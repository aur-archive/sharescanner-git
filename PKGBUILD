# Contributor: Yavor Stoychev <stoychev.yavor at gmail>

pkgname=sharescanner-git
pkgver=20110102
pkgrel=2
pkgdesc="The GNOME share scanner"
arch=('any')
url="https://sourceforge.net/projects/share-scanner/"
license=('GPL3')
depends=('python2' 'python2-pysmbc' 'python2-gobject')
makedepends=('git')
provides=()
conflicts=()
replaces=()
backup=()
options=(!emptydirs)
install=sharescanner.install

package() {
  git clone git://github.com/voran/sharescanner.git
  cd "$srcdir/sharescanner"
  python2 setup.py install --root="$pkgdir/" --optimize=1
}
