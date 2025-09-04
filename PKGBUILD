# Maintainer: Bouteiller a2n Alan <a2n.dev@pm.me>
pkgname=carnet-bin
pkgver=2.0.8
pkgrel=1
pkgdesc="Take notes without bloat"
arch=('x86_64')
url="https://github.com/results-may-vary-org/carnet"
license=('GPL')
depends=('cairo' 'desktop-file-utils' 'gdk-pixbuf2' 'glib2' 'gtk3' 'hicolor-icon-theme' 'libsoup3' 'pango' 'webkit2gtk-4.1')
options=('!strip' '!emptydirs')
install=${pkgname}.install
source_x86_64=("${url}/releases/download/v"${pkgver}"/carnet_"${pkgver}"_amd64.deb")
sha256sums_x86_64=('3aaba37aa3a538f05eee8b3a5c53a5d97fd7fda3e87f273884cc75fdedebeb3b')
package() {
  # Extract package data
  tar -xz -f data.tar.gz -C "${pkgdir}"
}
