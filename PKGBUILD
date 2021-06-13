# Maintainer: Damjan Georgievski <gdamjan@gmail.com>
pkgname=systemd-suspend-modules
pkgver=1.0
pkgrel=2
pkgdesc="Reload modules on suspend/hibernate with systemd"
arch=('any')
url="https://github.com/Necoro/systemd-suspend-modules"
license=('MIT')
depends=('systemd')
backup=('etc/suspend-modules.conf')
source=("suspend-modules")
md5sums=('3535221eaa42adf16548da7c57c8d76b')

package() {
    # Install files
    install -Dm755 "${srcdir}/suspend-modules" "${pkgdir}/usr/lib/systemd/system-sleep/suspend-modules"
    mkdir ${pkgdir}/etc/
    touch ${pkgdir}/etc/suspend-modules.conf
}
