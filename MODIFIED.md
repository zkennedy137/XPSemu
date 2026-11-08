# Modifications to xemu for XPSemu

This build is modified from xemu at base commit `ffa4943` (the xemu commit
the PS5 logs report as `ffa49432490a50eb42c0b9561374b615ccad6465`). It is
not the official xemu release. The changes are below. Each changed file keeps
xemu's GPL-2.0-or-later licence.

| File | Change |
|---|---|
| `system/vl.c` | A game image passed last on the command line is taken as the DVD, not as a disk. |
| `ui/xemu-input-ps5.c` | Holding the PS5 touchpad for three seconds asks for an exit. |
| `ui/xui/menubar.cc` | The UI thread acts on that exit request. |
| `ui/xui/dashboard.cc`, `ui/xui/dashboard.hh` | The PS5 dashboard: a game handed over by TotalEmu, discs in the drive, an Exit button on the System page, and return to TotalEmu through its helper. |
| `ps5/build-title.sh` | The PS5 link step; an opt-in `NO_PTHREAD_WRAP` switch, off by default. |
| `ps5/compat/libc_stubs.c` | Stub functions are marked weak so the PS5 C library can provide its own. |
