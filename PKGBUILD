# Maintainer: Bouteiller a2n Alan <a2n.dev@pm.me>
pkgname=tape-bin
appname=tape
pkgver=3.7.0
pkgrel=2
pkgdesc="Take notes without bloat"
arch=('x86_64')
url="https://github.com/results-may-vary-org/tape"
license=('GPL')
depends=('glibc' 'gtk3' 'webkit2gtk-4.1' 'desktop-file-utils' 'hicolor-icon-theme')
options=('!strip' '!emptydirs')
install=${pkgname}.install
source_x86_64=("${url}/releases/download/v"${pkgver}"/"${appname}"_"${pkgver}"_amd64.deb")
sha256sums_x86_64=('81bad868110b7f7938c6268eb8274b639c345cb7ac871bb4fdf498b8a489cc36')
package() {
  # Extract the deb package
  ar x "${appname}_${pkgver}_amd64.deb"

  # Extract package data
  tar -xz -f data.tar.gz -C "${pkgdir}"

  # Fix permissions
  chmod 755 "${pkgdir}/usr/bin/tape"
}
