# 🤖 ndroBot (Skyzoo Final Deployable)

![Skyzoo Bot](https://img.shields.io/badge/WhatsApp-Bot-green?style=for-the-badge&logo=whatsapp)
![Deploy](https://img.shields.io/badge/Deploy%20Ready-Heroku%20%7C%20Render-blueviolet?style=for-the-badge&logo=heroku)

Bot WhatsApp multi-fungsi + AI + musik + manajemen grup & pengguna.  
Disiapkan agar **langsung bisa di-deploy ke Heroku, Render, Docker, atau VPS** tanpa sentuhan manual.

---

## 🚀 Fitur Utama
- ✅ Tanya jawab AI (`!ai <pertanyaan>`) — ChatGPT API
- 🎵 Musik, anime, nonton, playlist
- 🛡️ Anti-link, virtex, blacklist/whitelist
- 📊 Statistik user & grup
- ❤️ Sistem favorit, top mingguan, profil user
- 💸 Donasi otomatis + QR dynamic (VIP)
- 🔧 Admin tools, owner panel, animasi menu interaktif

---

## 🔌 Deploy Langsung

### 💜 Heroku
[![Deploy to Heroku](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

> Gunakan file `Procfile`, `package.json`, dan `.env`

---

### 🔷 Render.com
Tambahkan repo ini di dashboard Render → pilih **type: Background Worker**.

```yaml
startCommand: node main.js
buildCommand: npm ci --omit=dev
```

---

### 🐳 Docker
```bash
docker build -t skyzoo .
docker run --env-file .env -v $(pwd)/session:/app/session skyzoo
```

---

### 💻 VPS (Ubuntu)
```bash
bash deploy.sh
```

---

## ⚙️ Konfigurasi ENV

Salin `.env.example` menjadi `.env`, isi seperti ini:

```
OPENAI_API_KEY=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
MONGO_URI=mongodb+srv://user:pass@cluster.mongodb.net/skyzoo
BOT_NUMBER=6285739419548
SESSION_ID=skyzoo-session
```

---

## 🙏 Credits
- WhatsApp Web.js
- OpenAI API
- Skyzoo / NdroBot base by [@NdroZuga27](https://github.com/NdroZuga27)---

## 📸 Tampilan Bot & Panel

### 🤖 Tampilan Menu Bot (WhatsApp)
<img src="https://telegra.ph/file/fb4f82c0b0a924e52f314.jpg" alt="Menu Bot" width="300"/>

### 🖥️ Tampilan Web Panel (mode dark + mobile)
<img src="https://telegra.ph/file/ccf8fd6ae8cb4ebf73dd2.jpg" alt="Web Panel Dark" width="300"/>

---

## 📊 Status & Informasi Tambahan

[![GitHub last commit](https://img.shields.io/github/last-commit/NdroZuga27/skyzoo-bot?style=flat-square)](https://github.com/NdroZuga27/skyzoo-bot)
[![GitHub repo stars](https://img.shields.io/github/stars/NdroZuga27/skyzoo-bot?style=flat-square)](https://github.com/NdroZuga27/skyzoo-bot/stargazers)
[![Uptime Robot status](https://img.shields.io/uptimerobot/status/m788027199-dfda49f3d6a74939ae60d3a9?style=flat-square)](https://stats.uptimerobot.com/XXXXX)
