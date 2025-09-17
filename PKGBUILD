# Maintainer: @zstg <zestig@duck.com>
pkgname=stratos-starship-hyprland-config
pkgver=1.0
pkgrel=5
pkgdesc="Starship configuration for StratOS Hyprland"
arch=('any')
license=('GPL3')
depends=(
    'starship'
)
conflicts=('stratos-starship-niri-config')
source=()
install=stratos-starship-config.install

prepare() {
    cp -r "$startdir/.config/" "$srcdir/"
}

package() {
    install -d "$pkgdir/etc/skel/.config"
    cp -r "$srcdir/.config/starship/" "$pkgdir/etc/skel/.config/"
    cp "$srcdir/.config/starship/tokyonight-dark/starship.toml" "$pkgdir/etc/skel/.config/starship.toml"
}
