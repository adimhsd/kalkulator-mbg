# Kalkulator MBG

🚀 **Kalkulator Mata Uang Galaksi (Galaxy Currency Calculator)** - A satirical currency converter that converts Indonesian Rupiah to "MBG Days" based on a fictional exchange rate.

> **1.200.000.000.000 Rupiah = 1 Hari MBG** ✨

## 📱 Fitur Utama

- ✅ **Konversi Rupiah ke MBG** - Masukkan jumlah rupiah dan dapatkan hasilnya dalam format hari, jam, menit, dan detik
- 🌓 **Dark Mode Support** - Toggle antara mode light dan dark dengan preferensi tersimpan di localStorage
- 📱 **Responsive Design** - Dioptimalkan untuk mobile dan desktop menggunakan Tailwind CSS
- 🎯 **Formatasi Input Otomatis** - Input rupiah secara otomatis diformat dengan pemisah ribuan (titik) sesuai standar Indonesia
- 🔢 **Presisi Tinggi** - Mendukung angka besar dengan presisi desimal hingga 12 angka di belakang koma

## 🛠️ Tech Stack

- **Frontend:** HTML5, Vanilla JavaScript, Tailwind CSS
- **Backend/Hosting:** Firebase Hosting
- **Build Tool:** Firebase CLI
- **Package Manager:** npm

## 📋 Prerequisites

- Node.js v14+ dan npm
- Firebase CLI (`npm install -g firebase-tools`)
- Akun Google untuk Firebase

## 🚀 Installation & Setup

1. **Clone Repository**
   ```bash
   git clone https://github.com/adimhsd/kalkulator-mbg.git
   cd kalkulator-mbg
   ```

2. **Install Dependencies**
   ```bash
   npm install
   ```

3. **Setup Firebase** (jika belum dikonfigurasi)
   ```bash
   firebase login
   firebase init
   ```

4. **Development Mode** (Opsional - untuk testing lokal)
   ```bash
   firebase emulators:start
   ```

5. **Deploy ke Firebase Hosting**
   ```bash
   npm run build  # (jika ada build process)
   firebase deploy
   ```

## 📖 Cara Menggunakan

1. **Masukkan Nominal**
   - Ketik jumlah uang dalam Rupiah pada input field
   - Angka otomatis akan diformat dengan pemisah ribuan (contoh: 1.000.000)

2. **Klik Tombol "Hitung"**
   - Aplikasi akan membagi nominal Anda dengan 1.2 triliun Rupiah per hari MBG
   - Hasil ditampilkan dalam format:
     - **Hari MBG** - Jumlah hari dalam satuan MBG
     - **Jam** - Setara dengan berapa jam
     - **Menit** - Setara dengan berapa menit
     - **Detik** - Setara dengan berapa detik
     - **Atau tepatnya** - Tampilan ringkas unit paling relevan

## 🧮 Rumus Kalkulasi

```
Hari MBG = Nominal Rupiah / 1.200.000.000.000
Jam = Hari MBG × 24
Menit = Jam × 60
Detik = Menit × 60
```

## 🎨 Desain & UI

- **Color Scheme:**
  - Biru Gelap: `#1e3a8a` (Primary)
  - Biru Terang: `#3b82f6` (Secondary)
  - Dark Background: `#0f172a`

- **Font:** Tailwind CSS Default (sans-serif)
- **Layout:** Mobile-first responsive design (max-width: 448px untuk optimal viewing)

## 📁 Project Structure

```
kalkulator-mbg/
├── index.html              # Main application file
├── package.json            # Dependencies & project metadata
├── firebase.json           # Firebase configuration
├── .firebaserc             # Firebase project settings
├── public/                 # Static assets for hosting
│   └── index.html         # Public folder index
├── node_modules/          # Dependencies (git-ignored)
├── .gitignore             # Git ignore rules
└── README.md              # This file
```

## 📝 Konfigurasi Firebase

File `firebase.json` mengatur:
- **Hosting Public Folder:** `public/`
- **Rewrites:** Semua request dialihkan ke `index.html` untuk SPA routing
- **Ignore Patterns:** Node modules, hidden files, dan Firebase config tidak diupload

## 🌐 Deployment

### Development
```bash
firebase serve
```

### Production
```bash
firebase deploy --only hosting
```

## 🔒 Environment & Security

- `.gitignore` mencakup:
  - `.firebase/` - Local Firebase cache
  - `.firebaserc` - Firebase project config (sensitive)
  - `node_modules/` - Dependencies
  - Local environment files

## ⚙️ Scripts

```json
{
  "dependencies": {
    "firebase": "^12.11.0"
  }
}
```

**Catatan:** Project ini adalah PWA sederhana tanpa build process. Firebase SDK dimuat dari CDN.

## 🎯 Konteks & Filosofi

**"Mata Uang Galaksi"** (MBG) adalah istilah satire yang digunakan dalam percakapan publik untuk menggambarkan skala anggaran besar yang sulit dibayangkan manusia normal. Kalkulator ini:

- Mengkonversi jumlah Rupiah besar ke unit "MBG" yang lebih absurd
- Membantu visualisasi skala uang yang sangat besar
- Edukasi & hiburan tentang notasi besar dalam pembahasan anggaran publik
- **Bukan kurs resmi** - Hanya perbandingan aritmatika satire

## 👨‍💻 Author & Credits

- **Developer:** [adi-muhamad.my.id](https://adi-muhamad.my.id)
- **Inspiration:** Percakapan publik tentang anggaran "mata uang galaksi"
- **Logo:** Badan Gizi Nasional (BGN)
- **Tagline:** "Dosen Sontoloyo" 🎓

## 📄 License

© 2026 BGN Lovers. All rights reserved.

## 🤝 Kontribusi

Kontribusi, issue reports, dan pull requests sangat diterima!

1. Fork repository
2. Buat feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to branch (`git push origin feature/AmazingFeature`)
5. Buat Pull Request

## 📞 Support

Untuk pertanyaan atau masalah, silakan buka [GitHub Issues](https://github.com/adimhsd/kalkulator-mbg/issues).

---

**Selamat menghitung MBG Anda! 🚀✨**
