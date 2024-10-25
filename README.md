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
