# Third-Party Notices for WineCX Distributables

WineCX Distributables builds and publishes macOS app bundles containing Wine binaries built from CrossOver source releases provided by CodeWeavers.

## Wine / CrossOver Source

- Component: Wine-compatible runtime built from CrossOver source releases.
- License: GNU Lesser General Public License, version 2.1 or later (`LGPL-2.1-or-later`), plus any additional licenses present in the upstream source archive.
- Upstream source page: `https://www.codeweavers.com/crossover/source`
- Source archive pattern used by this build repository: `https://media.codeweavers.com/pub/crossover/source/crossover-sources-<version>.tar.gz`
- Build scripts: `https://github.com/m5kro/winecx-dist`
- Modifications: This build does not modify Wine or CrossOver source code. It configures, compiles, stages, signs, and packages the upstream source into a macOS app bundle.

Each release should provide or link:

- The binary artifact: `winecx-<version>-osx64.tar.gz`.
- The corresponding source archive: `crossover-sources-<version>.tar.gz`.
- The LGPL license text: `COPYING.LIB`.
- Version-specific source/build information: `WINECX_SOURCE.md`.

## Build Dependencies

The GitHub Actions workflow installs build dependencies from Homebrew, including compiler/toolchain packages and libraries used by Wine's configure script. These dependencies remain under their respective upstream licenses.

No Homebrew dependency source code is modified by this repository.

## Trademark Notice

WineCX Distributables is not affiliated with, sponsored by, or endorsed by CodeWeavers. CrossOver is a CodeWeavers product/mark. Wine is a separate open-source project.