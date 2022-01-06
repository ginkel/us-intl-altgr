# Maintainer: Thilo-Alexander Ginkel <thilo@ginkel.com>

pkgname=kbd-us-intl-nodeadkeys
pkgver=1.0
pkgrel=0
pkgdesc="A US international keymap for the Linux virtual console that provides accented characters via Right-Alt / AltGr."
arch=('any')
license=('Apache')
source=("us-altgr-intl-nodeadkeys.map")
md5sums=('debb02e90977c203ca83c51c84adc060')

build() {
  gzip -f us-altgr-intl-nodeadkeys.map
}

package() {
  mkdir -p "$pkgdir/usr/share/kbd/keymaps/i386/qwerty"
  cp 'us-altgr-intl-nodeadkeys.map.gz' "$pkgdir/usr/share/kbd/keymaps/i386/qwerty/"
}
