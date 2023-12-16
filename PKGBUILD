
#Maintainer: MD MINAL HASAN RAJ MIM <minalhasan2@gmail.com>

pkgname=snigdhaos-brave-config
org=snigdhalinux
pkgver=1.0.0
pkgrel=1
pkgdesc="Snigdha OS Brave Config by minal hasan."
arch=('any')
license=("GPL")
url="https://github.com/$org/$pkgname"
depends=('brave-bin' 'gnome-keyring' 'profile-sync-daemon-brave')
source=("$pkgname.tar.gz"
        "psd.conf")
sha512sums=('SKIP'
            'SKIP')


package() {
  install -dm 755 "${pkgdir}/etc/skel/.config/BraveSoftware"
  install -dm 755 "${pkgdir}/etc/skel/.config/psd"

  cp -rf "${srcdir}/Brave-Browser" "${pkgdir}/etc/skel/.config/BraveSoftware/"
  cp -rf "${srcdir}/psd.conf" "${pkgdir}/etc/skel/.config/psd/"  
  
}
