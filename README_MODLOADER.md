# GPS Mod — GTA San Andreas (2004, offline)

Garis rute kuning menuju titik yang kamu tandai di map/radar, pakai sistem
pathfinding bawaan game sendiri (bukan garis lurus asal, tapi ngikut jalan).
Muncul otomatis saat kamu sedang di dalam kendaraan (bukan pesawat/heli/BMX)
dan ada target blip aktif di radar.

## Cara pasang (ModLoader)

1. Pastikan kamu sudah punya **ModLoader** (by Seemann) terpasang di folder
   utama GTA SA (tempat `gta_sa.exe` berada), dan ModLoader itu sendiri sudah
   bisa jalan (artinya kamu juga sudah punya ASI Loader di root game).
2. Buat folder baru di dalam `modloader/`, misalnya:
   `modloader/GPS-Mod/`
3. Taruh file `GPSMod.asi` ke dalam folder itu:
   `modloader/GPS-Mod/GPSMod.asi`
4. Jalankan game. Tandai lokasi tujuan di map seperti biasa, naik kendaraan,
   garis kuning bakal muncul di radar/minimap menuju titik itu.

Kalau ternyata versi ModLoader kamu tidak otomatis meng-load file `.asi` di
dalam subfoldernya (jarang terjadi, tapi beda versi beda perilaku), taruh
`GPSMod.asi` langsung di folder utama game (sebelah `gta_sa.exe`) sebagai
alternatif — itu pasti kebaca oleh ASI Loader.

## Catatan

- Ini mod visual murni (nambah elemen di radar/HUD), bukan cheat — gak ada
  perubahan ke stats/achievement.
- Dibuat dari contoh resmi "GPS" di Plugin-SDK (toolkit modding GTA komunitas),
  cuma warna garis & teksnya diubah jadi kuning.
