# DrownFi - WiFi Pentesting Tool

**DrownFi** adalah alat pentesting jaringan WiFi berbasis GUI untuk Linux, dirancang untuk membantu penguji keamanan mengevaluasi kerentanan jaringan nirkabel. Dibangun dengan **Python**, **PyQt5**, dan **Scapy**, DrownFi menghadirkan antarmuka dengan visualisasi serangan dan fitur-fitur seperti pemindaian jaringan, pengelolaan koneksi perangkat, serta serangan deauthentication dan ARP spoofing.

> ⚠️ **Peringatan Hukum:** Gunakan DrownFi hanya pada jaringan yang Anda miliki izin eksplisit. Penggunaan tanpa izin dapat melanggar hukum. Pengembang tidak bertanggung jawab atas penyalahgunaan alat ini.

---

## ✨ Fitur

- **Pemindaian Jaringan:** Deteksi perangkat dengan IP, MAC, dan vendor.
- **Lock/Unlock WiFi:** Putuskan semua koneksi dengan serangan deauthentication (butuh mode monitor).
- **Kelola Perangkat:** Disconnect/reconnect perangkat secara individu atau massal via ARP spoofing.
- **Tabel Perangkat:** Daftar perangkat dengan status koneksi dan vendor.
- **Grafik Serangan:** Visualisasi real-time aktivitas jaringan.
- **Antarmuka GUI:** Dark mode dengan ikon kustom.

---

## 🔧 Prasyarat

- **OS:** Linux (Debian/Ubuntu direkomendasikan)
- **WiFi Adapter:** Mendukung mode monitor & paket injeksi (chipset Atheros/Ralink direkomendasikan)
- **Akses Root:** Dibutuhkan untuk operasi jaringan

### Dependensi:
- Python 3.8+
- Paket Python: `scapy`, `pyqt5`, `netifaces`, `pandas`, `mac-vendor-lookup`, `matplotlib`
- Alat Tambahan: `aircrack-ng` (untuk mode monitor)

---

## ⚙️ Instalasi

# Kloning repositori
git clone https://github.com/frostyxsec/DrownFi.git
cd DrownFi

# (Opsional) Buat virtual environment
python3 -m venv venv
source venv/bin/activate

# Instal dependensi
pip install scapy pyqt5 netifaces pandas mac-vendor-lookup matplotlib

# Instal aircrack-ng
sudo apt update
sudo apt install aircrack-ng
