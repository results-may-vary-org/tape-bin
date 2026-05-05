# Maintainer: Bouteiller a2n Alan <a2n.dev@pm.me>
pkgname=tape-bin
appname=tape
pkgver=3.7.3
pkgrel=3
pkgdesc="Take notes without bloat"
arch=('x86_64')
url="https://github.com/results-may-vary-org/tape"
license=('GPL')
depends=('glibc' 'gtk3' 'webkit2gtk-4.1' 'desktop-file-utils' 'hicolor-icon-theme')
options=('!strip' '!emptydirs')
install=${pkgname}.install
source_x86_64=("${url}/releases/download/v"${pkgver}"/"${appname}"-gtk4_"${pkgver}"_amd64.deb")
sha256sums_x86_64=('820e367bdb45a3c6d593aeb42a11d524a6cde36955e2064753ed449794b4cdc4')
package() {
  # Extract the deb package
  ar x "${appname}-gtk4_${pkgver}_amd64.deb"

  # Extract package data (nfpm may use gz, xz, or zst compression)
  tar -xf data.tar.* -C "${pkgdir}"

  # Fix permissions
  chmod 755 "${pkgdir}/usr/bin/tape"
}
