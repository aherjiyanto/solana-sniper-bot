# solana-sniper-bot
⚡ NeuroMind V3 Titan - Solana Private RPC Sniper

Aplikasi Dashboard Sniper Solana berbasis Web yang dirancang untuk kecepatan eksekusi tinggi menggunakan infrastruktur Private RPC Node.

🛠️ Langkah-Langkah Instalasi (Runtut)

Ikuti panduan ini jika Anda ingin menjalankan aplikasi di komputer lokal (Localhost):

1. Persiapan Lingkungan

Pastikan Anda sudah menginstal:

Node.js (Versi 18 ke atas disarankan)

npm atau yarn

2. Inisialisasi Proyek React

Buka terminal/CMD Anda, lalu jalankan perintah berikut:

npx create-react-app titan-sniper-bot
cd titan-sniper-bot


3. Instalasi Dependensi

Aplikasi ini membutuhkan library ikon dan framework CSS:

# Instal Ikon
npm install lucide-react

# Instal Tailwind CSS (Wajib untuk Tampilan)
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p


4. Konfigurasi Tailwind

Edit file tailwind.config.js di folder proyek Anda dan tambahkan jalur konten:

/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src/**/*.{js,jsx,ts,tsx}"],
  theme: {
    extend: {},
  },
  plugins: [],
}


Tambahkan direktif Tailwind ke dalam file ./src/index.css:

@tailwind base;
@tailwind components;
@tailwind utilities;


5. Memasukkan Kode Aplikasi

Buka file src/App.js.

Hapus semua kode bawaan di dalamnya.

Copy & Paste kode NeuroMind V3 Titan yang saya berikan sebelumnya ke dalam file tersebut.

6. Menjalankan Aplikasi

npm start


Buka http://localhost:3000 di browser Anda.

🚀 Cara Menggunakan Fitur Sniper

Hubungkan Private RPC:
Dapatkan API Key dari Helius atau QuickNode. Masukkan URL RPC di bagian Private Gateway pada aplikasi.

Setel Risk Management:
Atur Position Size, Stop Loss, dan Take Profit di panel Execution Engine.

Aktifkan Auto-Sniper:
Klik tombol Play pada Engine Status. Bot akan mulai memantau Live Feed koin yang aman (SAFE) untuk dieksekusi.

Pantau Latensi:
Pastikan bar Node Latency berwarna hijau (di bawah 150ms) untuk memastikan kecepatan transaksi maksimal.

⚠️ Disclaimer (Peringatan)

Trading koin di jaringan Solana (terutama Memecoins) memiliki risiko sangat tinggi. Alat ini dibuat untuk membantu analisis teknis dan kecepatan eksekusi. Gunakan modal yang siap Anda lepaskan (Risk Capital). Kami tidak bertanggung jawab atas kerugian finansial yang terjadi.

📄 Lisensi

MIT License - Bebas digunakan dan dikembangkan untuk tujuan edukasi.
