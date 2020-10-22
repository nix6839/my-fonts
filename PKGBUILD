# Maintainer: Nix <nix6839@protonmail.ch>

pkgname=my-fonts
pkgver=1
pkgrel=1
pkgdesc="Nix's using fonts"
arch=('any')
url='https://gitlab.com/nix6839/my-fonts'
license=('custom:OFL')
provides=('ttf-font')
conflicts=('ttf-d2coding'
           'ttf-nanum')
source=('fonts.tar.gz'
        'd2coding-fonts-LICENSE'
        'nanum-fonts-LICENSE')
sha256sums=('069fedca91ef6cfb9239da5b63d4fa6d1cead52d3d3456e46e252ddc96c6d755'
            '9f409ab80b85e75a99037046ff4a8880fb7ea701a1aae58b5ac3059775f75a38'
            'c6038f6740085ea48901ac510c13184a24ddc522859322600bb8ccb6a33d85ab')

package() {
  install -Dm 644 fonts/D2Coding/D2Coding/D2Coding-Ver1.3.2-20180524.ttc "$pkgdir"/usr/share/fonts/d2coding/D2Coding.ttc
  install -Dm 644 fonts/D2Coding/D2CodingNerdFont/D2Coding-Ver1.3.2-20180524-NerdFont.ttf "$pkgdir"/usr/share/fonts/d2coding/D2CodingNerdFont.ttf
  install -Dm 644 fonts/D2Coding/D2CodingNerdFont/D2CodingBold-Ver1.3.2-20180524-NerdFont.ttf "$pkgdir"/usr/share/fonts/d2coding/D2CodingBoldNerdFont.ttf
  install -Dm 644 fonts/Nanum/*/*.ttf -t "$pkgdir"/usr/share/fonts/nanum/

  install -Dm 644 d2coding-fonts-LICENSE "$pkgdir"/usr/share/licenses/d2coding-fonts/LICENSE
  install -Dm 644 nanum-fonts-LICENSE "$pkgdir"/usr/share/licenses/nanum-fonts/LICENSE
}
