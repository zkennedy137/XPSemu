# XPSemu - third-party components

XPSemu is built from xemu (GPL-2.0-or-later, `COPYING-GPL-2.0`). Its changes
are listed in `MODIFIED.md`. The licence texts for xemu's own bundled
components are in `licenses/`.

Components built for the PS5 (versions as pinned in `ps5/deps/build-deps.sh`):

| Component | Version | Licence | Notice file |
|---|---|---|---|
| libcurl | 8.16.0 | curl | `licenses/third-party/curl-COPYING` |
| mbedTLS | 3.6.4 | Apache-2.0 or GPL-2.0 (dual) | `licenses/third-party/mbedtls-LICENSE` |
| zlib | 1.3.1 | zlib | `licenses/third-party/zlib-LICENSE` |
| GLib | 2.84.4 | LGPL-2.1 | `licenses/third-party/glib-COPYING` |
| libiconv | 1.18 | LGPL-2.0-or-later | `licenses/third-party/libiconv-COPYING.LIB` |
| libpcap | 1.10.5 | BSD-3-Clause | `licenses/third-party/libpcap-LICENSE` |
| libsamplerate | 0.2.2 | BSD-2-Clause | `licenses/third-party/libsamplerate-COPYING` |
| libslirp | 4.9.1 | BSD-3-Clause | `licenses/third-party/libslirp-COPYRIGHT` |
| pixman | 0.44.2 | MIT | `licenses/third-party/pixman-COPYING` |
| SDL3 | 3.2.24 | zlib | `licenses/third-party/SDL3-LICENSE.txt` |

Bundled data:

| Item | Licence | Notice file |
|---|---|---|
| Blank Xbox HDD image (`ps5/blank-hdd/xbox_hdd.qcow2`) | MIT (xemu-dashboard, Ryzee119) | `licenses/third-party/xemu-dashboard-blank-hdd-MIT.txt` |
| Patch catalog (`ps5/patch-catalog.tsv`) | NOT YET CONFIRMED: the source repository has no licence | - |
| Box art name list (`ps5/libretro-xbox-boxarts.txt`) | NOT YET CONFIRMED: the source repository has no licence | - |

The two data items above must be resolved before a release is published.
