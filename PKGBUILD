# This file was generated by GoReleaser. DO NOT EDIT.
# Maintainer: Mark Cornick <mcornick@mcornick.com>

pkgname='mpg-bin'
pkgver=1.1.1
pkgrel=1
pkgdesc='Mark's Password Generator'
url='https://mcornick.com/mpg/'
arch=('aarch64' 'armv6h' 'i686' 'x86_64')
license=('MIT')
provides=('mpg')
conflicts=('mpg')

source_aarch64=("${pkgname}_${pkgver}_aarch64.tar.gz::https://github.com/mcornick/mpg/releases/download/v1.1.1/mpg_1.1.1_linux_arm64.tar.gz")
sha256sums_aarch64=('d6845d843da2e2dcacd6456afc61a4efa88a44072b0c9db0fdb5d79607172d78')

source_armv6h=("${pkgname}_${pkgver}_armv6h.tar.gz::https://github.com/mcornick/mpg/releases/download/v1.1.1/mpg_1.1.1_linux_armv6.tar.gz")
sha256sums_armv6h=('e48754b22ebbf248f243d832d75c88da09f386ea9f4e73a0338514b7381684b2')

source_i686=("${pkgname}_${pkgver}_i686.tar.gz::https://github.com/mcornick/mpg/releases/download/v1.1.1/mpg_1.1.1_linux_386.tar.gz")
sha256sums_i686=('21ffc4f1c553eb0ac13a516a40b004dd0e7a9c7b553702c3a1aaaed283aa6efb')

source_x86_64=("${pkgname}_${pkgver}_x86_64.tar.gz::https://github.com/mcornick/mpg/releases/download/v1.1.1/mpg_1.1.1_linux_amd64.tar.gz")
sha256sums_x86_64=('3f5cdae1838d2f7d7511c352833d5932bb8e0cd80c677eaa8459cbae7c7a4411')

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
