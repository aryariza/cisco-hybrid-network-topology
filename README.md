# Hybrid Network Topology for 3 Buildings

Proyek ini adalah simulasi desain infrastruktur jaringan komputer yang menghubungkan tiga gedung berbeda menggunakan model **Topologi Hybrid** (kombinasi Star dan Mesh). Simulasi dibuat menggunakan **Cisco Packet Tracer** sebagai bagian dari tugas evaluasi jaringan.

## Arsitektur Jaringan

Proyek ini menerapkan konsep redundansi dan efisiensi melalui dua lapisan topologi:

1.  **Topologi Star (Intra-Gedung):** Setiap gedung menggunakan switch pusat yang menghubungkan semua PC dan server. Ini memastikan manajemen kabel yang rapi dan kemudahan deteksi kerusakan perangkat lokal.
2.  **Topologi Mesh (Inter-Gedung):** Antar router gedung dihubungkan secara Full Mesh. Jika salah satu jalur antar gedung terputus, data tetap bisa dikirim melalui jalur cadangan melalui router gedung lain.



## Komponen & Teknologi
- **Perangkat:** Router, Switch, Server, dan PC (End-devices).
- **Konektivitas:** Menggunakan kabel otomatis dan konfigurasi IP address untuk setiap subnet gedung.
- **Redundansi:** Protokol routing memastikan *zero downtime* jika terjadi kegagalan link antar router.

## Kelebihan Desain
- **Skalabilitas:** Mudah untuk menambah perangkat baru di setiap gedung tanpa mengganggu gedung lain.
- **Reliabilitas:** Koneksi Mesh antar gedung memastikan jaringan tetap berjalan meskipun ada jalur yang mati.
- **Performa:** Distribusi beban data yang seimbang di setiap gedung.

## Cara Menjalankan
1. Download dan instal **Cisco Packet Tracer**.
2. Clone repositori ini:
   ```bash
   git clone [https://github.com/aryariza/cisco-hybrid-network-topology.git](https://github.com/aryariza/cisco-hybrid-network-topology.git)
