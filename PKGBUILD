# Maintainer: Archiv8 <archiv8@artisteducator.com>
# Contributor: Archiv8 <archiv8@artisteducator.com>


_upstreamname="PDVinstall_2_5_Linux"
# _langname=""
# _relname=""
#_partname=""
#_cvsname=""


# pkgbase=
pkgname="paye-desktop-viewer"
pkgver=2.5
pkgrel=1
# epoch=
pkgdesc="PAYE Desktop Viewer is an application from HM Revenue and Customs (HMRC) that allows you to view, search and sort large numbers of employee tax codes and notices."
arch=("any")
url="https://www.gov.uk/paye-online/desktop-viewer"
license=("GPLv2")
# groups=()
depends=("jre")
# optdepends=()
makedepends=("unzip")
# checkdepends=()
# provides=()
# conflicts=()
# replaces=()
# backup=()
# options=()
# install=
changelog="CHANGELOG.md"
source=(
"http://www.hmrc.gov.uk/gds/payerti/tools/pdv/$_upstreamname.zip"
)
md5sums=('1fd596a50e03da978f7c226e53012a85')

noextract=("PDVinstall_2_5_Linux.zip")
# validpgpkeys=()

# prepare () {}

# build() {}

# check() {}

package() {
  ls -al

  # If files and folders from paye-desktop-viewer-2.5.zip exist, remove them
  [[ -f PDVinstall.bin ]] && rm PDVinstall.bin
  [[ -f README_LINUX.txt ]] && rm README_LINUX.txt
  [[ -d __MACOSX ]] && rm -rf __MACOSX

ls -al

  unzip "$_upstreamname.zip"

  ls -al

  sh ./PDVinstall.bin -i silent

}
