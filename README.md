# openwrt-sync-time
Script sederhana untuk mengatasi tanggal openwrt reset ke 2015 setelah listrik mati.

> `Note: script ini tidak membuat waktu otomatis realtime setelah listrik mati! Tetapi hanya mendekati waktu terakhir sebelum mati listrik, sehingga tetap bisa terhubung ke internet.`

Pastikan terhubung ke internet sebelum mengeksekusi script dibawah
### Install

```bash
curl -s https://raw.githubusercontent.com/utoro/openwrt-sync-time/main/sync-time | bash -s install
```

Karena file `rc.local` saya seringkali ikut kereset setelah mati listrik, maka ada opsi untuk install ke startup
```bash
curl -s https://raw.githubusercontent.com/utoro/openwrt-sync-time/main/sync-time | bash -s install startup
```
> `Note: Pilih salah satu! Jangan install keduanya.
`
### Uninstall

```bash
curl -s https://raw.githubusercontent.com/utoro/openwrt-sync-time/main/sync-time | bash -s uninstall
```
