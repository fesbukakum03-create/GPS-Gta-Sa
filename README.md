# GPS-Gta-Sa

GPS mod untuk GTA San Andreas PC (2004, offline) — garis rute **kuning**
menuju titik yang kamu tandai di map, mengikuti jalan sungguhan (pathfinding
bawaan game), dirender di radar/minimap. Dibangun dari contoh resmi "GPS" di
[Plugin-SDK](https://github.com/DK22Pac/plugin-sdk), cuma warna garisnya
diubah jadi kuning.

## Download

Langsung ambil dari folder **[`result/GPS-Mod/`](result/GPS-Mod)** di repo
ini — tinggal buka `GPSMod.asi`, klik **Download raw file**. File ini
otomatis ter-update setiap ada perubahan (di-build & di-commit balik oleh
GitHub Actions).

## Cara pasang

Lihat [README_MODLOADER.md](README_MODLOADER.md).

## Struktur repo

- `patches/GPS_Main.cpp` — source plugin (modifikasi warna dari contoh GPS
  resmi Plugin-SDK)
- `external/plugin-sdk` — submodule toolkit modding (tidak diubah, source
  kita di-copy menimpanya saat build di CI)
- `.github/workflows/build.yml` — pipeline GitHub Actions yang compile
  otomatis jadi `.asi` setiap push
- `README_MODLOADER.md` — instruksi pasang ke ModLoader

## Build lokal (opsional, kalau punya Windows + Visual Studio)

Lihat langkah-langkah di `.github/workflows/build.yml` — generate project
pakai `external/plugin-sdk/tools/premake/premake5.exe`, lalu compile pakai
MSBuild/Visual Studio.
