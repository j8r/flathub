# Flatpak for Play!

## Install

1. [Set up Flatpak](https://www.flatpak.org/setup/)

2. Install xemu from [Flathub](https://flathub.org/apps/details/org.purei.Play)

`flatpak install -y org.purei.Play`

3. Run xemu

`flatpak run org.purei.Play`

To uninstall: `flatpak uninstall -y org.purei.Play`

## Build

The `flatpak-builder` package is required.

- Install the SDK

`flatpak install org.freedesktop.Platform/x86_64/21.08 org.kde.Sdk/x86_64/5.15-21.08`

- Build Play!

`flatpak-builder --user --install --force-clean build-dir app.xemu.xemu.yml`
