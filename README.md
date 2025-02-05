# flatpak-sideband
<BR>Flatpak builds of Sideband (https://github.com/markqvist/Sideband)
<BR>This build connects to the internet to download all Rust dependencies for maturin and cryptography which isn't Flatpak standard.
<BR>
<BR>Build:
<BR>clear && flatpak-builder --jobs=3 --ccache --disable-rofiles-fuse --force-clean build-dir io.unsigned.sideband.yml
<BR>
<BR>Install:
<BR>clear && flatpak-builder --user --install --jobs=3 --ccache --disable-rofiles-fuse --force-clean --delete-build-dirs --disable-download build-dir io.unsigned.sideband.yml
