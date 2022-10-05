# Flatpak for Vita3K

## Install

1. [Set up Flatpak](https://www.flatpak.org/setup/)

2. Install Vita3K from [Flathub](https://flathub.org/apps/details/org.vita3k.Vita3K)

`flatpak install -y org.vita3k.Vita3K`

3. Run Vita3K

`flatpak run org.vita3k.Vita3K`

To uninstall: `flatpak uninstall -y org.vita3k.Vita3K`

## Build

The `flatpak-builder` package is required.

- Install the SDK

`flatpak install org.freedesktop.Platform/x86_64/23.08 org.freedesktop.Sdk/x86_64/23.08`

- Build Vita3K

`flatpak-builder --user --install --force-clean build-dir org.vita3k.Vita3K.yml`
