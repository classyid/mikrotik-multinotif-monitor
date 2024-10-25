## README.md:
```markdown
# MikroTik Multi-Platform Notification Monitor

Monitor status RouterOS Anda dengan notifikasi multi-platform yang dikirim ke WhatsApp, Telegram dan Email. Script ini memberikan informasi lengkap tentang kondisi router secara real-time.

## 🚀 Fitur Utama
- Monitoring sistem router (CPU, Memory, Uptime)
- Informasi perangkat (Board, RouterOS version)
- Status koneksi WAN & traffic monitoring
- Statistik DNS dan DHCP
- Notifikasi multi-platform:
  - WhatsApp
  - Telegram
  - Email

## 📋 Informasi yang Ditampilkan
- Info Router:
  - Nama router
  - Model perangkat
  - Versi RouterOS
  - IP Public
  - CPU & Memory usage
  - DNS cache status
- DHCP Status:
  - Total perangkat terdaftar
  - Jumlah perangkat aktif
- Status WAN:
  - Status koneksi
  - Total download/upload

## 📦 Persyaratan
- RouterOS v6.49 atau lebih baru
- Akses API WhatsApp Gateway
- Bot Telegram
- Konfigurasi SMTP untuk email

## ⚙️ Konfigurasi
1. Setting API WhatsApp:
   ```routeros
   :local apikey "YOUR-API-KEY"
   :local sender "YOUR-SENDER"
   ```

2. Setting Bot Telegram:
   ```routeros
   :local botToken "YOUR-BOT-TOKEN"
   :local chatId "YOUR-CHAT-ID"
   ```

3. Setting Email:
   ```routeros
   /tool e-mail
   set address=smtp.gmail.com from="router@domain.com" password="pass" port=587
   ```

## 📥 Instalasi
1. Copy script ke router
2. Sesuaikan konfigurasi (API keys, tokens, email)
3. Jalankan script untuk test
4. Schedule script untuk monitoring rutin

## 🔄 Penggunaan
Script dapat dijalankan:
- Manual melalui terminal
- Terjadwal via scheduler
- Trigger events tertentu

## 📝 Contoh Output
```
------- ROUTER STATUS -------

>> INFO ROUTER:
Nama      : PPANet-Router
Board     : RB5009
RouterOS  : 7.11.2
Public IP : > 202.x.x.x
...

>> DHCP STATUS:
Total     : > 25 devices
Active    : > 12 devices
...
```

## 🤝 Kontribusi
Kontribusi selalu diterima. Silakan buat pull request atau laporkan issues.

## 📜 Lisensi
MIT License - Silakan gunakan dan modifikasi sesuai kebutuhan.

## 🙏 Credits
- PPANet Network Solution
- Komunitas MikroTik Indonesia
```

