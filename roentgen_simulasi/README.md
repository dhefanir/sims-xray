# Simulasi Pesawat Roentgen

Aplikasi ini terdiri dari dua bagian:
1. Panel Kontrol (Streamlit)
2. Simulasi Visual (p5.js)

## Cara Menjalankan Aplikasi

### 1. Menjalankan Panel Kontrol (Streamlit)

1. Buka terminal pertama
2. Pastikan Python dan Streamlit sudah terinstall
3. Install dependencies yang diperlukan:
```bash
pip install streamlit
```
4. Jalankan aplikasi Streamlit:
```bash
streamlit run app.py
```
5. Panel kontrol akan terbuka di browser (biasanya di http://localhost:8501)

### 2. Menjalankan Server Simulasi (p5.js)

1. Buka terminal kedua
2. Jalankan server Python untuk folder web:
```bash
cd web
python -m http.server 8000
```
3. Server simulasi akan berjalan di http://localhost:8000

## Cara Penggunaan

1. Buka Panel Kontrol di http://localhost:8501
2. Atur parameter yang diinginkan (kV, mA, waktu)
3. Klik tombol "Buka Simulasi"
4. Simulasi akan terbuka di tab baru
5. Untuk mengubah parameter, kembali ke tab Panel Kontrol

## Struktur Folder

- `app.py` - Aplikasi Panel Kontrol (Streamlit)
- `web/` - Folder simulasi p5.js
  - `index.html` - Halaman simulasi
  - `sketch.js` - Kode simulasi p5.js 