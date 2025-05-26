# QC Progressive Report Web Aplication (Design)

## 📋 Deskripsi
Aplikasi web untuk laporan produksi harian Departemen Quality Control - Cream Processing PT. Anugrah Mitra Maju. Sistem ini memungkinkan 3 shift kerja untuk melakukan input data secara berkesinambungan dalam satu hari produksi.

## 🎯 Fitur Utama
- **Multi-Shift Interface**: Tiga tab shift dengan jam kerja berbeda
  - 🌅 **Shift 1**: 07:00-15:00 (Pagi)
  - 🌤️ **Shift 2**: 15:00-23:00 (Sore) 
  - 🌙 **Shift 3**: 23:00-07:00 (Malam)

- **Progressive Data Entry**: Shift berikutnya dapat melanjutkan data dari shift sebelumnya
- **PDF Generation**: Generate laporan dalam format PDF
- **Data Security**: Sistem verifikasi untuk mencegah manipulasi data
- **Responsive Design**: Optimized untuk desktop dan mobile

## 🔒 Sistem Keamanan

### Kode Verifikasi
- Setiap shift memiliki kode verifikasi unik dan rahasia
- Mencegah shift lain memalsukan data shift tertentu
- Harus diisi sebelum generate PDF

### Kode Produksi
- Format berisi: hari-tanggal-tahun-shift-nama_shift
- Contoh: `010151A` 
- Mencegah input data dari hari yang berbeda
- Memastikan kontinuitas produksi harian

## 🔄 Alur Kerja

### Shift 1 (Pagi)
- Memulai laporan harian baru
- Input data produksi awal
- Generate PDF untuk diteruskan ke shift berikutnya

### Shift 2 (Sore)
- **Opsi 1**: Upload PDF dari Shift 1 untuk melanjutkan data
- **Opsi 2**: Memulai laporan baru jika produksi dimulai dari shift 2
- Generate PDF gabungan (Shift 1 + 2) atau PDF baru

### Shift 3 (Malam)
- **Opsi 1**: Upload PDF dari shift sebelumnya untuk melanjutkan
- **Opsi 2**: Memulai laporan baru jika produksi dimulai dari shift 3
- Generate PDF final untuk satu hari produksi

## 📊 Data yang Dikumpulkan

### Storage Data
- Top Gap Storage BSC (cm)
- Top Gap Storage MCP (cm)

### Ballmill BSC
- Jumlah Start Batch dalam Ballmill (kg)
- Jumlah Proses BSC Hari Ini (kg)
- Jumlah End Batch dalam Ballmill (kg)
- Jumlah Pemakaian (kg)

### Ballmill MCP
- Jumlah Start Batch dalam Ballmill (kg)
- Jumlah Proses MCP Hari Ini (kg)
- Jumlah End Batch dalam Ballmill (kg)
- Jumlah Pemakaian (kg)

### Informasi Tambahan
- Keterangan shift (kendala/catatan penting)
- Kode produksi
- Kode verifikasi shift

## 🛠️ Teknologi

### Frontend (Current - Design Only)
- **HTML5**: Struktur aplikasi
- **CSS3**: Styling dengan responsive design
- **JavaScript**: Interaksi dasar UI (tab switching)

### Backend (In Development)
- PDF generation functionality
- Data persistence
- File upload handling
- Verification system

## 📁 Struktur File
```
qc-progressive-report/
├── index.html          # Main HTML file
├── style.css           # Styling
├── README.md           # Documentation
```

## 🚀 Cara Penggunaan

### Setup
1. Clone repository ini
2. Buka `index.html` di web browser
3. Pilih shift yang sesuai dengan jam kerja

### Input Data Shift 1
1. Masukkan kode produksi
2. Isi semua data storage dan ballmill
3. Tambahkan keterangan jika diperlukan
4. Masukkan kode verifikasi shift 1
5. Generate PDF

### Input Data Shift 2/3
1. **Jika melanjutkan**: Upload PDF dari shift sebelumnya
2. **Jika memulai baru**: Langsung isi form
3. Lengkapi semua data yang diperlukan
4. Masukkan kode verifikasi yang sesuai
5. Generate PDF

## ⚠️ Status Pengembangan

### ✅ Selesai (Design Phase)
- UI/UX Design
- Responsive layout
- Form structure
- Tab navigation
- CSS styling

### 🔄 Dalam Pengembangan (Backend Team)
- PDF generation functionality
- File upload processing
- Data validation
- Verification system
- Data persistence
- Progressive data merging

## 📱 Kompatibilitas
- ✅ Chrome/Chromium
- ✅ Firefox
- ✅ Safari
- ✅ Edge
- ✅ Mobile browsers

## 🔮 Roadmap
- [ ] Backend API development
- [ ] Database integration
- [ ] User authentication
- [ ] Data export features
- [ ] Historical report viewing
- [ ] Email notification system

## 👥 Tim Pengembangan
- **Frontend/Design**: Current contributor
- **Backend/Functionality**: Departemen IT (In Progress)
- **Quality Control**: PT. Anugrah Mitra Maju

## 📞 Kontak
Untuk pertanyaan teknis atau feedback:
- diwangkararevan@gmail.com

---

## 📝 Catatan Penting
- Aplikasi ini masih dalam tahap **DESIGN ONLY**
- Fungsionalitas backend sedang dikembangkan oleh tim terpisah
- UI/UX sudah final dan siap untuk implementasi backend
- Tidak ada data yang tersimpan dalam versi current ini

## 🤝 Kontribusi
Saat ini proyek ini dalam fase design completion. Kontribusi backend akan dihandle oleh departemen IT internal.

---
*Last updated: May 2025*
