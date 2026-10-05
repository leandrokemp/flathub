# Tibia Flatpak

Tibia MMORPG client.

Verdana fonts are included in the package. 

This community-provided package is not verified by, affiliated with, or supported by CipSoft GmbH.

## Building Locally

### Prerequisites
- `flatpak` installed
- `flatpak-builder` installed

### Build

```bash
# Initialize Flatpak runtime (first time only)
flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo

# Build the package
flatpak-builder --user --install --force-clean build-dir flatpak/com.tibia.client.yml

# Run
flatpak run com.tibia.client
