# Maintainer: Bouteiller a2n Alan <a2n.dev@pm.me>
pkgname=cassette-bin
pkgver=2.1.6
pkgrel=1
pkgdesc="Take notes without bloat"
arch=('x86_64')
url="https://github.com/results-may-vary-org/cassette"
license=('GPL')
depends=('cairo' 'desktop-file-utils' 'gdk-pixbuf2' 'glib2' 'gtk3' 'hicolor-icon-theme' 'libsoup3' 'pango' 'webkit2gtk-4.1')
options=('!strip' '!emptydirs')
install=${pkgname}.install
source_x86_64=("${url}/releases/download/v"${pkgver}"/cassette_"${pkgver}"_amd64.deb")
sha256sums_x86_64=('61435d5a9db670b9d2dffab157bf221a0d57d7069a7383b7454067d6b3a2d800')
package() {
  # Extract package data
  tar -xz -f data.tar.gz -C "${pkgdir}"
}
