# Maintainer: sataa <supersonicsataa@gmail.com>

pkgname=rp-alt-grub
pkgver=1.0
pkgrel=1
pkgdesc='An alternate GRUB theme using the Rosé Pine palette'
arch=('any')
url="https://github.com/FieryMewtwo/rp-alt-grub"
license=('MIT')
depends=('grub')
source=("${url}"/archive/refs/tags/1.0.tar.gz)
sha256sums=('b71f0851b5ebc85420d8ad67385d1348f0472f081d9020ab083ea594dc78ca21')

package() {
    cd "rp-alt-grub-1.0"
    install -d "${pkgdir}/usr/share/grub/themes"
    cp -R "${srcdir}/${pkgname}-${pkgver}" "${pkgdir}/usr/share/grub/themes/"
    install -Dm 644 "license" "${pkgdir}/usr/share/licenses/${pkgname}/license"
    install -Dm 644 "readme.md" "${pkgdir}/usr/share/doc/${pkgname}/readme.md"
    }
