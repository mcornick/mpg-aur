# This file was generated by GoReleaser. DO NOT EDIT.
# Maintainer: Mark Cornick <mcornick@mcornick.com>

pkgname='mpg-bin'
pkgver=1.2.4
pkgrel=1
pkgdesc='Mark's Password Generator'
url='https://mcornick.com/mpg/'
arch=('aarch64' 'armv6h' 'i686' 'x86_64')
license=('MIT')
provides=('mpg')
conflicts=('mpg')

source_aarch64=("${pkgname}_${pkgver}_aarch64.tar.gz::https://github.com/mcornick/mpg/releases/download/v1.2.4/mpg_1.2.4_linux_arm64.tar.gz")
sha256sums_aarch64=('8163409a3a763debef391cc9f92ad930433328263570775688a3f79f0c390e27')

source_armv6h=("${pkgname}_${pkgver}_armv6h.tar.gz::https://github.com/mcornick/mpg/releases/download/v1.2.4/mpg_1.2.4_linux_armv6.tar.gz")
sha256sums_armv6h=('8bd90b1201dd7a2d1120bc7d2804f92fedc1e605f3a16cb42b3d04e5a9fc813b')

source_i686=("${pkgname}_${pkgver}_i686.tar.gz::https://github.com/mcornick/mpg/releases/download/v1.2.4/mpg_1.2.4_linux_386.tar.gz")
sha256sums_i686=('5163b47e205886988fbf95932c74b117ca00627820640b1138109f67f6f1305f')

source_x86_64=("${pkgname}_${pkgver}_x86_64.tar.gz::https://github.com/mcornick/mpg/releases/download/v1.2.4/mpg_1.2.4_linux_amd64.tar.gz")
sha256sums_x86_64=('0c50f5b956c9c7e042681d0b4688e3b8f072cab18cffcebf0978c1cfa8a7793d')

package() {
  install -Dm755 "./mpg" "${pkgdir}/usr/bin/mpg"
  install -Dm644 "./LICENSE" "${pkgdir}/usr/share/licenses/mpg/LICENSE"
  mkdir -p "${pkgdir}/usr/share/bash-completion/completions/"
  mkdir -p "${pkgdir}/usr/share/zsh/site-functions/"
  mkdir -p "${pkgdir}/usr/share/fish/vendor_completions.d/"
  install -Dm644 "./completions/mpg.bash" "${pkgdir}/usr/share/bash-completion/completions/mpg"
  install -Dm644 "./completions/mpg.zsh" "${pkgdir}/usr/share/zsh/site-functions/_mpg"
  install -Dm644 "./completions/mpg.fish" "${pkgdir}/usr/share/fish/vendor_completions.d/mpg.fish"
  install -Dm644 "./manpage/mpg.1" "${pkgdir}/usr/share/man/man1/mpg.1"
}
