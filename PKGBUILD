# Maintainer : pixy <raeonz@gmail.com>
# Contributor: pixy <raeonz@gmail.com>

pkgname=chrome-pepper-flashplugin
pkgver=11.3.31.208
pkgrel=1
pkgdesc="Google Chrome's Pepper Flashplugin (64-bit) for google-chrome stable and beta channels"
arch=('x86_64')
url="http://blogs.adobe.com/flashplayer/2010/03/improved_flash_player_support.html"
optdepends=("pulseaudio-alsa: For pulseaudio users")
license=('custom')
install=pepper.install
source=(http://dl.google.com/dl/linux/direct/google-chrome-unstable_current_${arch}.rpm)

package() {
  install -dm755 "$pkgdir/usr/lib/PepperFlash"
  for i in opt/google/chrome/PepperFlash/*; do install -m644 "$i" "$pkgdir/usr/lib/PepperFlash"; done
}

md5sums=('a179be0fcff7df83b7151d4468331a04')
