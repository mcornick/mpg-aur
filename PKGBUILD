# This file was generated by GoReleaser. DO NOT EDIT.
# Maintainer: Mark Cornick <mcornick@mcornick.com>

pkgname='mpg-bin'
pkgver=1.2.2
pkgrel=1
pkgdesc='Mark's Password Generator'
url='https://mcornick.com/mpg/'
arch=('aarch64' 'armv6h' 'i686' 'x86_64')
license=('MIT')
provides=('mpg')
conflicts=('mpg')

source_aarch64=("${pkgname}_${pkgver}_aarch64.tar.gz::https://github.com/mcornick/mpg/releases/download/v1.2.2/mpg_1.2.2_linux_arm64.tar.gz")
sha256sums_aarch64=('80097c1f5a2f89082b9a27c5aa259c3b6fbf99635ba02dddf78f130df59ed5e8')

source_armv6h=("${pkgname}_${pkgver}_armv6h.tar.gz::https://github.com/mcornick/mpg/releases/download/v1.2.2/mpg_1.2.2_linux_armv6.tar.gz")
sha256sums_armv6h=('b471a2d989bb9671430914e3539e2c07f782e3d88ea4517e9af1340294907b3f')

source_i686=("${pkgname}_${pkgver}_i686.tar.gz::https://github.com/mcornick/mpg/releases/download/v1.2.2/mpg_1.2.2_linux_386.tar.gz")
sha256sums_i686=('7239e435709e52504651afca7648e99994dfa5ef088388a64298423c1acd9773')

source_x86_64=("${pkgname}_${pkgver}_x86_64.tar.gz::https://github.com/mcornick/mpg/releases/download/v1.2.2/mpg_1.2.2_linux_amd64.tar.gz")
sha256sums_x86_64=('e82075c952fe0692b7429408956f0da5d613dccf6b061a5fd98b13d63f25019c')

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
