# This file was generated by GoReleaser. DO NOT EDIT.
# Maintainer: Mark Cornick <mcornick@mcornick.com>

pkgname='mpg-bin'
pkgver=1.1.0
pkgrel=1
pkgdesc='Mark's Password Generator'
url='https://mcornick.com/mpg/'
arch=('aarch64' 'armv6h' 'i686' 'x86_64')
license=('MIT')
provides=('mpg')
conflicts=('mpg')

source_aarch64=("${pkgname}_${pkgver}_aarch64.tar.gz::https://github.com/mcornick/mpg/releases/download/v1.1.0/mpg_1.1.0_linux_arm64.tar.gz")
sha256sums_aarch64=('cf94d431b788a71e4299c67e39304bf1e1af04c5cb8d0d51159a97b99c0db6a2')

source_armv6h=("${pkgname}_${pkgver}_armv6h.tar.gz::https://github.com/mcornick/mpg/releases/download/v1.1.0/mpg_1.1.0_linux_armv6.tar.gz")
sha256sums_armv6h=('4d7c015aac252b7e28eb5e0a91e23d5cc778e4db0e7f954b71d3836f40009a8d')

source_i686=("${pkgname}_${pkgver}_i686.tar.gz::https://github.com/mcornick/mpg/releases/download/v1.1.0/mpg_1.1.0_linux_386.tar.gz")
sha256sums_i686=('4ec944e2d9ed3a678e4f485ba664a3de390a35ff2e017964cd7b6d916e111ef6')

source_x86_64=("${pkgname}_${pkgver}_x86_64.tar.gz::https://github.com/mcornick/mpg/releases/download/v1.1.0/mpg_1.1.0_linux_amd64.tar.gz")
sha256sums_x86_64=('6cec71530824dd6bb928bacd7e21b73138a2aadcd4f286fe49855a35d86ef864')

package() {
  install -Dm755 "./mpg" "${pkgdir}/usr/bin/mpg"
  install -Dm644 "./LICENSE" "${pkgdir}/usr/share/licenses/mpg/LICENSE"
  mkdir -p "${pkgdir}/usr/share/bash-completion/completions/"
  mkdir -p "${pkgdir}/usr/share/zsh/site-functions/"
  mkdir -p "${pkgdir}/usr/share/fish/vendor_completions.d/"
  install -Dm644 "./completions/mpg.bash" "${pkgdir}/usr/share/bash-completion/completions/mpg"
  install -Dm644 "./completions/mpg.zsh" "${pkgdir}/usr/share/zsh/site-functions/_mpg"
  install -Dm644 "./completions/mpg.fish" "${pkgdir}/usr/share/fish/vendor_completions.d/mpg.fish"
  install -Dm644 "./manpages/mpg.1" "${pkgdir}/usr/share/man/man1/mpg.1"
}
