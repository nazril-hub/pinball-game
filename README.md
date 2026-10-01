# ðŸŽ¯ BOLA MASA DEPAN â€” Arcade Pinball BK

> **Media Bimbingan & Konseling Interaktif Berbasis Gamifikasi Arcade Pinball**  
> *"Putar bolanya, temukan arahnya, tentukan langkahnya."*  
> Memfasilitasi eksplorasi karir dan studi lanjut siswa melalui dinamika kelompok, tantangan misi refleksi, dan penyusunan Lembar Future Journey.

---

## ðŸ•¹ï¸ Fitur Utama

1. **Arcade Pinball Physics Engine**:
   - Simulasi fisika 2D (kecepatan, pantulan bumper interaktif, pasak logam/pegs, lorong peluncur/chute dengan pegas dinamis).
   - Pengatur daya peluncur bola (*Launch Force*) dengan tombol Spasi atau tombol luncur.
2. **5 Zona Eksplorasi Bimbingan Konseling**:
   - **Zona 01 â€” Kenali Aku** (Mengenali diri, potensi, bakat autentik).
   - **Zona 02 â€” Jelajah Pilihan** (Ragam jurusan, politeknik, vokasi & karir).
   - **Zona 03 â€” Timbang Pilihan** (Faktor realitas: biaya, prospek, restu orang tua).
   - **Zona 04 â€” Pilih Arah** (Menentukan kompas awal eksplorasi prodi).
   - **Zona 05 â€” Langkahku** (Action plan mikro 7 hari ke depan bersama Guru BK).
3. **25 Misi Reflektif & Panduan Diskusi**:
   - Setiap zona memiliki 5 kartu misi bervariasi dengan panduan fasilitator bagi dinamika kelompok.
4. **Dinamika Kelompok & Fasilitasi**:
   - Multi-player switcher (Pemain 1 s/d 6).
   - Poin apresiasi kelompok (*Group Points*) dengan efek konfeti.
   - Timer hitung mundur sesi bimbingan (45:00) dengan kontrol Start / Pause / Reset.
5. **Lembar Future Journey (Siap Cetak)**:
   - Formulir refleksi terintegrasi dengan penyimpanan otomatis di browser lokal (*LocalStorage*).
   - Format print-friendly otomatis (hanya mencetak lembar kerja Future Journey).

---

## ðŸ”’ Proteksi Logika & Keamanan (Logic Protection)

- **Bundle Terenkripsi**: Seluruh data zona, kartu misi, panduan konseling, dan algoritma fisika arcade pinball telah dienkripsi menggunakan *Base64 string table* dan diobfuskasi ke dalam [`assets/app.min.js`](assets/app.min.js).
- **Pembersihan File Sumber**: File mentah (`pinball.html` dan `backup_dev/`) secara otomatis diabaikan oleh [`.gitignore`](.gitignore) sehingga tidak akan terekspos ke repositori GitHub.

---

## ðŸš€ Panduan Push ke GitHub & Deploy ke Vercel

### Repository GitHub
Repository ini terhubung ke:
```bash
https://github.com/nazril-hub/pinball-game.git
```

Untuk memperbarui repository:
```bash
git add .
git commit -m "update: README and documentation"
git push origin main
```

---

### Deploy ke Vercel

1. Buka [vercel.com](https://vercel.com) dan login dengan akun GitHub Anda.
2. Klik **Add New...** â†’ **Project**.
3. Pilih repository **`pinball-game`**.
4. Pilih Framework Preset: **Other**.
5. Klik **Deploy**. Aplikasi akan langsung online dalam beberapa detik!

---

## ðŸ“ Struktur File Project

```
pinball_project/
â”œâ”€â”€ .gitignore              # Memfilter file mentah / source code asli
â”œâ”€â”€ vercel.json             # Konfigurasi deployment & security headers Vercel
â”œâ”€â”€ index.html              # Entry point produksi (Vercel ready)
â”œâ”€â”€ README.md               # Dokumentasi project & deployment
â”œâ”€â”€ assets/
â”‚   â””â”€â”€ app.min.js          # Bundle logika & engine pinball terenkripsi
â””â”€â”€ backup_dev/             # (Lokal) Backup file sumber mentah
```

---

## ðŸ› ï¸ Penggunaan Lokal

Cukup buka file `index.html` langsung di browser, atau jalankan menggunakan Live Server di VS Code. Seluruh fitur (simulasi fisika canvas, audio effects, timer, confetti, dan penyimpanan lokal) berjalan 100% di browser tanpa ketergantungan server/database eksternal.