# Contributing to Main Roleplay GTA SA Radar Mod

Terima kasih telah tertarik untuk berkontribusi pada mod radar GTA SA untuk server SAMP "Main Roleplay". Berikut adalah panduan langkah demi langkah untuk membantu Anda dalam proses kontribusi.

## Tools yang Diperlukan
Sebelum memulai, pastikan Anda telah mengunduh dan menginstal tools berikut:
- **Magic TXD** - [Download](https://www.mixmods.com.br/2017/01/magic-txd-criar-editar-txd/)
- **GTA Radar Creator** - [Download](https://forum.mixmods.com.br/f307-utilities/t6093-iii-vc-sa-lcs-vcs-gta-radar-creator-merge-split)
- **GIMP** - [Download](https://www.gimp.org/downloads/)

## Cara Berkontribusi

1. **Clone repository ini**
   ```sh
   git clone https://github.com/flxzor/mainroleplay-radar
   cd mainroleplay-radar
   ```

2. **Unduh tools yang diperlukan** (lihat daftar di atas).

3. **Buka file `radar.xcf` dalam GIMP**
   - File ini berada di dalam folder repository.
   - Edit gambar untuk menambahkan nama jalan yang kurang.
   - Setelah selesai, simpan sebagai `.xcf` dan export sebagai `.png`.
   - Simpan hasilnya di folder `Merged` di dalam repo.

4. **Gunakan GTA Radar Creator**
   - Buka GTA Radar Creator.
   - Masukkan folder `Merged` ke dalam GTA Radar Creator.
   - Jalankan `Merged To Splitted.bat`.
   - Ketik `512` saat diminta.
   - Tunggu hingga proses selesai.

5. **Gunakan Magic TXD untuk membangun TXD**
   - Buka Magic TXD.
   - Pilih tab `Tools` > `Mass Build`.
   - Pilih directory `Splitted` dari GTA Radar Creator sebagai sumber.
   - Pilih directory `Splitted` dalam repository sebagai tujuan.
   - Tunggu hingga proses selesai.

6. **Salin hasilnya ke folder tujuan**
   - Setelah selesai, salin file `radar01.txd` hingga `radar143.txd` ke folder `Main Roleplay Radar Map`.

7. **Commit dan push perubahan ke repository**
   ```sh
   git add .
   git commit -m "Deskripsi perubahan"
   git push origin main
   ```

## Selesai
Terima kasih telah berkontribusi pada mod radar GTA SA untuk Main Roleplay! Jika ada pertanyaan, jangan ragu untuk bertanya melalui issue atau diskusi pada repository ini.

