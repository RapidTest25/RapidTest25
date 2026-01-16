# 📋 Instruksi Setup GitHub Profile

## Langkah-langkah Setup Profile README:

### 1️⃣ Buat Repository Khusus Profile

1. Buka [GitHub](https://github.com/new)
2. Buat repository baru dengan nama **sama persis dengan username GitHub Anda**
   - Contoh: Jika username Anda `johndoe`, buat repo bernama `johndoe`
3. ✅ Centang "Public"
4. ✅ Centang "Add a README file"
5. Klik "Create repository"

---

### 2️⃣ Edit README.md

1. Buka repository yang baru dibuat
2. Klik file `README.md`
3. Klik tombol pensil (Edit) di kanan atas
4. Copy isi dari file `README.md` yang sudah saya buatkan
5. **PENTING: Ganti semua yang perlu diganti:**

#### Yang WAJIB Diganti:

```markdown
# Ganti ini dengan informasi Anda:

[Your Name]           → Nama lengkap Anda
yourusername          → Username GitHub Anda (di semua tempat!)
your.email@gmail.com  → Email Anda
yourportfolio.com     → URL portfolio Anda (jika ada)
yourdiscord           → Username Discord Anda
```

#### Contoh Penggantian:

**SEBELUM:**
```markdown
# Hi Everyone, 👋 I'm [Your Name]!

![Profile views](https://komarev.com/ghpvc/?username=yourusername&color=blueviolet)
```

**SESUDAH:**
```markdown
# Hi Everyone, 👋 I'm Budi Santoso!

![Profile views](https://komarev.com/ghpvc/?username=budisantoso&color=blueviolet)
```

---

### 3️⃣ Sesuaikan Konten

#### A. Bagian "About Me"
Edit deskripsi Anda sendiri:
```markdown
## 🚀 About Me

[Tulis tentang diri Anda, passion, dan goals Anda di sini]
```

#### B. Bagian "Technologies & Tools"
Hapus/tambah sesuai yang Anda kuasai:
- Jika tidak pakai Laravel, hapus badge Laravel
- Jika pakai Java, tambahkan badge Java
- Lihat daftar lengkap badges di: [shields.io](https://shields.io)

#### C. Bagian "Currently Learning"
Update dengan yang sedang Anda pelajari:
```markdown
## 🌱 Currently Learning

- 📚 Apa yang sedang Anda pelajari
- 🎨 Skill atau teknologi baru
```

#### D. Bagian "Featured Projects"
Ganti dengan repository terbaik Anda:
```markdown
[![Project 1](https://github-readme-stats.vercel.app/api/pin/?username=USERNAMEMU&repo=NAMA_REPO_1&theme=tokyonight&hide_border=true)](https://github.com/USERNAMEMU/NAMA_REPO_1)
```

#### E. Bagian "Connect with Me"
Update semua link social media:
```markdown
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/USERNAME_LINKEDIN_MU)
[![Instagram](https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://instagram.com/USERNAME_IG_MU)
```

---

### 4️⃣ Customize Theme GitHub Stats

Pilih tema favorit Anda untuk GitHub stats. Ganti `theme=tokyonight` dengan salah satu:

#### 🎨 Popular Themes:
- `radical`
- `dark`
- `merko`
- `gruvbox`
- `tokyonight`
- `onedark`
- `cobalt`
- `synthwave`
- `highcontrast`
- `dracula`
- `prussian`
- `monokai`
- `vue`
- `vue-dark`
- `shades-of-purple`
- `nightowl`
- `buefy`
- `blue-green`
- `algolia`
- `great-gatsby`
- `darcula`
- `bear`
- `solarized-dark`
- `solarized-light`
- `chartreuse-dark`
- `nord`
- `gotham`
- `material-palenight`
- `graywhite`
- `vision-friendly-dark`
- `ayu-mirage`
- `midnight-purple`
- `calm`
- `flag-india`
- `omni`
- `react`
- `jolly`
- `maroongold`
- `yeblu`
- `blueberry`
- `slateorange`
- `kacho_ga`

**Contoh perubahan:**
```markdown
<!-- Dari -->
theme=tokyonight

<!-- Menjadi -->
theme=radical
```

---

### 5️⃣ Optional: Tambahan Keren

#### A. Snake Animation (Contribution Snake)
1. Buat file `.github/workflows/snake.yml` di repository profile Anda
2. Copy paste code berikut:

```yaml
name: Generate Snake

on:
  schedule:
    - cron: "0 0 * * *"
  workflow_dispatch:

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v2
      - uses: Platane/snk@master
        id: snake-gif
        with:
          github_user_name: GANTI_DENGAN_USERNAME_MU
          gif_out_path: dist/github-contribution-grid-snake.gif
          svg_out_path: dist/github-contribution-grid-snake.svg
      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

3. Ganti `GANTI_DENGAN_USERNAME_MU` dengan username GitHub Anda
4. Commit dan tunggu beberapa menit
5. Snake animation akan muncul di profil Anda!

#### B. Trophy Stats
Tambahkan di README:
```markdown
<div align="center">
  
[![trophy](https://github-profile-trophy.vercel.app/?username=yourusername&theme=onedark&no-frame=true&row=1&column=7)](https://github.com/ryo-ma/github-profile-trophy)

</div>
```

#### C. Typing SVG
Tambahkan animated typing text:
```markdown
[![Typing SVG](https://readme-typing-svg.herokuapp.com?font=Fira+Code&pause=1000&color=F75C7E&width=435&lines=Full+Stack+Developer;Always+learning+new+things;Love+to+code+and+create)](https://git.io/typing-svg)
```

Customize text di parameter `lines`:
- Pisahkan setiap baris dengan `;`
- Gunakan `+` untuk spasi

---

### 6️⃣ Testing & Preview

1. **Sebelum commit**, preview terlebih dahulu:
   - Klik tab "Preview" saat edit
   - Pastikan semua link benar
   - Pastikan username sudah diganti semua

2. **Setelah yakin**, klik "Commit changes"

3. **Cek hasilnya**:
   - Buka profil GitHub Anda
   - README akan muncul di bagian atas profile

---

### 7️⃣ Troubleshooting

#### ❌ Stats tidak muncul?
- Pastikan username benar (case-sensitive)
- Tunggu beberapa menit (API perlu waktu)
- Cek apakah repository Anda public

#### ❌ Profile views tidak terupdate?
- Counter butuh waktu untuk update
- Pastikan URL username benar

#### ❌ Badge tidak muncul?
- Cek URL badge
- Pastikan connection internet stabil
- Beberapa service mungkin slow, refresh setelah beberapa saat

---

## 🎨 Customization Tips:

### Warna Badge
Ganti warna dengan kode hex:
```markdown
?color=blueviolet    → Warna ungu biru
?color=brightgreen   → Hijau terang
?color=ff69b4        → Pink
?color=00a8ff        → Biru
```

### Style Badge
```markdown
?style=flat-square   → Kotak flat
?style=for-the-badge → Badge tebal (recommended)
?style=flat          → Flat sederhana
?style=plastic       → Plastic style
?style=social        → Social media style
```

---

## 📚 Resources & Inspirasi:

- **GitHub Stats:** https://github.com/anuraghazra/github-readme-stats
- **Shields.io:** https://shields.io
- **Skill Icons:** https://github.com/tandpfun/skill-icons
- **Typing SVG:** https://github.com/DenverCoder1/readme-typing-svg
- **Snake Animation:** https://github.com/Platane/snk
- **Awesome README:** https://github.com/abhisheknaiidu/awesome-github-profile-readme

---

## ✅ Checklist Final:

- [ ] Repository profile sudah dibuat (nama = username)
- [ ] Semua `yourusername` sudah diganti
- [ ] Semua `[Your Name]` sudah diganti
- [ ] Link social media sudah benar
- [ ] Technology badges sesuai skill
- [ ] Featured projects sudah di-update
- [ ] Preview sudah dicek
- [ ] Commit dan push ke GitHub
- [ ] Profil GitHub dicek hasilnya

---

## 🎉 Selamat!

Profil GitHub Anda sekarang sudah menarik dan profesional! 

**Tips terakhir:**
- 📝 Update README secara berkala
- 🚀 Tambah project baru ke featured section
- 📊 Pantau stats Anda
- 💡 Cari inspirasi dari profile developer lain
- 🌟 Yang terpenting: Buat project berkualitas!

**Good luck dengan GitHub journey Anda!** 🚀✨
