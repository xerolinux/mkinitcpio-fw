# Maintainer: LinusDierheimer <Linus@Dierheimer.de>

pkgname=mkinitcpio-fw
pkgver=1.6.0
pkgrel=1
pkgdesc="Optional firmware for the default linux kernel to get rid of the annoying 'WARNING: Possibly missing firmware for module:' messages"
arch=("any")
url="https://github.com/xerolinux/mkinitcpio-fw"
license=("GPL")

#see https://wiki.archlinux.org/title/mkinitcpio#Possibly_missing_firmware_for_module_XXXX
depends=(
    "aic94xx-firmware"
    "ast-firmware"
    "linux-firmware-atheros"
    "linux-firmware-broadcom"
    "linux-firmware-cirrus"
    "linux-firmware-intel"
    "linux-firmware-marvell"
    "linux-firmware-mediatek"
    "linux-firmware-mellanox"
    "linux-firmware-nfp"
    "linux-firmware-other"
    "linux-firmware-qcom"
    "linux-firmware-qlogic"
    "linux-firmware-realtek"
    "linux-firmware-whence"
    "linux-firmware-qlogic"
    "linux-firmware-bnx2x"
    "linux-firmware-liquidio"
    "linux-firmware-mellanox"
    "linux-firmware-nfp"
    "upd72020x-fw"
    "wd719x-firmware"
)
optdepends=(
  "mkinitcpio: build the initramfs"
  "linux: default linux preset"
)
source=(
    mkinitcpio-firmware.hook
)
sha512sums=(0a04b74bbaf7f2e38b6d54214c09c55f00db00e4266c3c970040cbe20c8d2102f536c14279a32c8faa1503dcd8e39f13f79a5332ab023d3b46e36e43912cfe88)

package() {
    install -Dm644 "mkinitcpio-firmware.hook" "$pkgdir/usr/share/libalpm/hooks/$pkgname.hook"
}
