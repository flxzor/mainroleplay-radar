# Table of Contents

- [Contributing to Main Roleplay Radar Mod - ID](#contributing-to-main-roleplay-radar-mod---id)
  - [Tools yang Diperlukan](#tools-yang-diperlukan)
  - [Cara Berkontribusi](#cara-berkontribusi)
  - [Selesai](#selesai)
- [Contributing to Main Roleplay GTA SA Radar Mod - EN](#contributing-to-main-roleplay-gta-sa-radar-mod---en)
  - [Required Tools](#required-tools)
  - [How to Contribute](#how-to-contribute)
  - [Done](#done)

---

# Contributing to Main Roleplay Radar Mod - ID

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

---

# Contributing to Main Roleplay GTA SA Radar Mod - EN

Thank you for your interest in contributing to the GTA SA radar mod for the SAMP "Main Roleplay" server. Below is a step-by-step guide to help you with the contribution process.

## Required Tools
Before you begin, make sure you have downloaded and installed the following tools:
- **Magic TXD** - [Download](https://www.mixmods.com.br/2017/01/magic-txd-criar-editar-txd/)
- **GTA Radar Creator** - [Download](https://forum.mixmods.com.br/f307-utilities/t6093-iii-vc-sa-lcs-vcs-gta-radar-creator-merge-split)
- **GIMP** - [Download](https://www.gimp.org/downloads/)

## How to Contribute

1. **Clone this repository**
   ```sh
   git clone https://github.com/flxzor/mainroleplay-radar
   cd mainroleplay-radar
   ```

2. **Download the required tools** (see the list above).

3. **Open the `radar.xcf` file in GIMP**
   - This file is located in the repository folder.
   - Edit the image to add missing street names.
   - Once done, save it as `.xcf` and export it as `.png`.
   - Save the result in the `Merged` folder within the repository.

4. **Use GTA Radar Creator**
   - Open GTA Radar Creator.
   - Insert the `Merged` folder into GTA Radar Creator.
   - Run `Merged To Splitted.bat`.
   - Enter `512` when prompted.
   - Wait for the process to complete.

5. **Use Magic TXD to build TXD**
   - Open Magic TXD.
   - Select the `Tools` tab > `Mass Build`.
   - Choose the `Splitted` directory from GTA Radar Creator as the source.
   - Choose the `Splitted` directory in the repository as the destination.
   - Wait for the process to complete.

6. **Copy the results to the target folder**
   - Once done, copy the `radar01.txd` to `radar143.txd` files into the `Main Roleplay Radar Map` folder.

7. **Commit and push changes to the repository**
   ```sh
   git add .
   git commit -m "Description of changes"
   git push origin main
   ```

## Done
Thank you for contributing to the GTA SA radar mod for Main Roleplay! If you have any questions, feel free to ask via issues or discussions in this repository.

