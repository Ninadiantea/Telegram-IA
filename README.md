# Telegram AI Bot Multi User API Key

Bot Telegram AI (OpenAI) yang memungkinkan setiap user input API Key-nya sendiri.  
Sudah ada tombol menu rapi, jawaban AI mudah di-copy paste, siap deploy ke Railway.

## Fitur
- Bot Telegram AI (GPT-3.5, GPT-4, dsb)
- Setiap user simpan API Key sendiri (privat)
- Inline menu: 🔑 Set API Key, 🗑️ Hapus API, 📄 Panduan, 📝 Riwayat Chat
- Jawaban AI dalam format code block (mudah di-copy)
- Siap deploy ke Railway

## Cara Deploy

1. **Clone repo ke Railway (atau lokal):**
2. **Set environment variable:**
   - `BOT_TOKEN` = token dari BotFather
   - (Tidak perlu set OpenAI API Key, karena tiap user input sendiri)
3. **Install dependencies & run:**
   ```bash
   npm install
   npm start
   ```
4. **Tambahkan webhook/long polling sesuai kebutuhan Railway.**

## Struktur File

- `index.js` - Source code utama bot
- `package.json` - Daftar dependensi
- `.env.example` - Contoh environment variable
- `.gitignore` - Agar `.env` & `node_modules/` tidak ikut ke repo

## Panduan Penggunaan

- `/start` untuk menampilkan menu utama dan tombol
- Klik 🔑 **Set API Key** lalu masukkan API Key OpenAI (format: sk-xxx)
- Langsung chat ke bot, jawaban AI akan muncul dalam format mudah di-copy
- Pilih 🗑️ **Hapus API** untuk menghapus API key kamu
- Pilih 📝 **Riwayat Chat** untuk melihat 5 chat terakhir

---

**Happy hacking!**
