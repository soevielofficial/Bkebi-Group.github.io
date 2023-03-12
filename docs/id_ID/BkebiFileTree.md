# Pengantar Dokumen Bkebi

| **nama file/nama folder** | **penjelasan**            |
|:-----------------:|:------------:                     |
| BKEBI-ISFREE-NOT4SALE.LIC | Berkas Lisensi            |
| injector\.exe     | Program injektor Bkebi            |
| libstdimpact\.dll | Berkas .dll Bkebi                 |
| tp_files          | Berkas kustomisasi teleport       |
| themes            | Folder Tema                       |
| cfg\.ini          | Konfigurasi injektor              |
| cfg\.json         | Berkas konfigurasi Bkebi          |
| imgui\.ini        | Posisi tampilan internal Bkebi    |

Disarankan untuk mencadangkan dan menyimpan file `cfg.json`. File ini tidak hanya berisi konfigurasi Bkebi, tetapi juga tanda titik selesai.
Penulis secara pribadi menggunakan file BAT di bawah ini untuk memulai, dan akan menyalin dan mencadangkan dua versi. Itu dapat disalin dan diberi nama "start.bat" dan ditempatkan di direktori program Bkebi.

```cmd
@echo off
set rootPath=%cd%
echo %date%%time%

copy /Y cfg.json.backup cfg.json.backup2
copy /Y cfg.json cfg.json.backup
start injector.exe
```
