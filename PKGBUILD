# Contributor: Justin Davis <jrcd83@gmail.com>
pkgname= 'prankm'
pkgver=  '0.01'
pkgrel=  '1'
pkgdesc= "Parallel pinging mirrorlist ranker for pacman"
arch=   ('any')
license=('PerlArtistic' 'GPL')
options=('!emptydirs')
depends=('perl-anyevent-fastping')
url=     'http://github.com/juster/prankm'
source= ("http://gigithub.com/juster/prankm/tarball/v${pkgver}")

build() {
  cd "$srcdir"
  pod2man prankm | gzip -c --best > prankm.8.gz
  install -D prankm      "${pkgdir}/usr/sbin/prankm"
  install -D prankm.8.gz "${pkgdir}/usr/share/man8/prankm.8.gz"
}

# Local Variables:
# mode: shell-script
# sh-basic-offset: 2
# End: