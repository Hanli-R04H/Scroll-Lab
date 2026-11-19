# Scroll Lab

Repositori latihan mandiri untuk mendalami berbagai teknik *scroll* modern menggunakan HTML & CSS secara modular dan terpisah per konsep.

## Struktur File

* **Tahap 1 — Vertical Scroll & Sticky:** `vertical.html` & `vertical.css`
* **Tahap 2 — Horizontal Scroll:** `horizontal.html` & `horizontal.css`
* **Tahap 3 — Parallax Effect:** `parallax.html` & `parallax.css`

---

## Ringkasan Pembelajaran

### 1. Vertical Scroll & Sticky (`vertical.html` & `vertical.css`)
* **Smooth Scroll & Jarak Aman:** Menggunakan `scroll-behavior: smooth` agar perpindahan saat klik *anchor link* (`#id`) terasa halus, dipadukan dengan `scroll-margin-top` agar posisi berhenti punya jarak aman dari *navbar* atas.
* **Sticky Element:** Menggunakan `position: sticky` dengan `top` sesuai kebutuhan, serta `align-items: flex-start` pada *flex container* agar elemen tidak ikut meregang penuh dan punya ruang untuk menempel saat konten di sebelahnya di-*scroll*.
* **Scroll Snap:** Menggunakan `scroll-snap-type` dan `scroll-snap-align` untuk membantu menyelaraskan posisi berhenti *scroll* pada *section*.

### 2. Horizontal Scroll (`horizontal.html` & `horizontal.css`)
* **Wadah Menyamping:** Menggunakan `display: flex` dan `overflow-x: auto` agar item tersusun horizontal dan dapat digeser ke samping.
* **Mencegah Item Gepeng:** Menggunakan `flex-shrink: 0` pada item/kartu agar ukuran lebarnya tetap terjaga sesuai aturan meski jumlah item melebihi lebar layar.
* **Horizontal Snap & Bersihkan Scrollbar:** Mengombinasikan `scroll-snap-type: x mandatory` + `scroll-snap-align: start` untuk perhentian rapi per kartu, serta menyembunyikan *scrollbar* bawaan agar tampilan lebih bersih.

### 3. Parallax Effect (`parallax.html` & `parallax.css`)
* **Ilusi Kedalaman Latar Belakang:** Menggunakan `background-attachment: fixed` bersama `background-position: center` dan `background-size: cover` agar latar belakang terasa bergerak lebih lambat/terkunci relatif terhadap lapisan konten yang di-*scroll*.
* **Kontras & Transisi Visual:** Menambahkan lapisan `linear-gradient` tipis di atas gambar latar bila diperlukan agar teks lebih terbaca dan kontras antarlapisan terasa jelas.

---

## Catatan
Fokus utama repositori ini adalah memahami cara kerja tiap properti CSS secara bertahap dan terpisah sebelum diterapkan ke *project* web yang lebih besar.
