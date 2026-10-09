# ITQSHHB Teacher's Hub — Fasa 1

Portal statik, mesra mudah alih untuk pautan perkhidmatan warga pendidik. Tiada pangkalan data, maklumat pelajar, keputusan disiplin atau pengiraan markah dalam fasa ini.

## Struktur produk

- **Laporan Kes Disiplin** — laporan salah laku pelajar untuk perhatian dan tindakan Hal Ehwal Pelajar.
- **Kemajuan Hafazan Al-Quran** — laporan perkembangan hafazan, bacaan atau perkara berkaitan Al-Quran seseorang pelajar.
- **Kemajuan Akademik** — laporan perkembangan, pencapaian atau keperluan sokongan akademik seseorang pelajar.
- **Laporan Aktiviti Pelajar** — borang laporan terperinci untuk diisi oleh Ketua Bahagian (HOD) atau penganjur aktiviti.
- **Kalendar Aktiviti** — pautan kepada kalendar Institut.
- **Bahagian Pembangunan Pelajar** — laman rasmi BPP.

Semua perkhidmatan berada pada satu halaman utama. Pautan kosong dipaparkan sebagai **Pautan Belum Tersedia** tanpa butang yang rosak.

Pautan laporan disiplin, hafazan, akademik, aktiviti pelajar dan kalendar aktiviti menggunakan URL yang diberikan.

## Gantikan URL borang

Edit `config.js` untuk mengemas kini pautan `disiplin`, `hafazan`, `akademik`, `aktiviti` atau `kalendar`. Pautan BPP juga dikonfigurasi di sana. Pautan yang kosong dipaparkan sebagai **Pautan Belum Tersedia** tanpa butang yang rosak.

Contoh:

```js
links: {
  disiplin: "https://docs.google.com/forms/d/e/FORM_ID/viewform",
  hafazan: "https://docs.google.com/forms/d/e/FORM_ID/viewform",
  akademik: "https://docs.google.com/forms/d/e/FORM_ID/viewform",
  aktiviti: "https://docs.google.com/forms/d/e/FORM_ID/viewform",
  kalendar: "https://script.google.com/macros/s/DEPLOYMENT_ID/exec",
  bpp: "https://hep-itqshhb.github.io/bpp-itq/"
}
```

## Logo

Logo ITQSHHB yang dibekalkan disimpan pada `logo-itqshhb.png`. Untuk menggantikannya, letakkan fail logo rasmi yang diluluskan di lokasi sama dengan nama yang sama. Jangan gunakan logo rekaan atau tiruan.

## Uji secara setempat

Buka `index.html` dalam pelayar, atau jalankan pelayan statik daripada folder ini. Semak paparan pada lebar 320 px, telefon, tablet dan desktop; tab fokus papan kekunci; pautan kosong; pautan BPP; dan pautan HTTPS yang telah dikonfigurasi.

## Persediaan GitHub Pages

Portal ini statik dan tidak memerlukan pangkalan data atau build step. Untuk penerbitan yang benar-benar berasingan daripada BPP, gunakan repositori Teacher's Hub khusus, aktifkan Pages daripada branch `main` dan folder root, kemudian semak URL Pages yang diberikan GitHub.

### Konfigurasi penting sebelum pelancaran

1. Pastikan URL borang dan kalendar masih aktif.
2. Gunakan repositori Teacher's Hub yang berasingan daripada laman BPP.

Tiada credential diperlukan untuk laman statik ini. Google Forms dan kalendar mengurus akses serta data di sistem masing-masing. Jika kawalan akses warga sekolah diwajibkan, gunakan penyelesaian Google Workspace yang disahkan dan jangan menganggap pautan tersembunyi atau kod pelayar sebagai kawalan keselamatan.
