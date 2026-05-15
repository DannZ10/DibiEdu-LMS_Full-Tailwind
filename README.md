# 🎓 Tugas Frontend: DibiEdu - Learning Management System (LMS)

Halo Kak! Ini adalah hasil pengerjaan tugas konversi UI untuk antarmuka web **DibiEdu**. Fokus utama saya di tugas ini adalah memindahkan styling dari HTML/CSS mentah menjadi Tailwind CSS, sambil memastikan layout-nya tetap responsif dan konsisten.

## 📝 Catatan Pengerjaan

Tantangan terbesar di tugas ini adalah menstruktur ulang layout bawaan agar cocok dengan pola *utility classes* dari Tailwind, terutama pas ngatur *behavior* di berbagai device. Tujuannya biar *user* yang buka lewat HP, tablet, atau desktop tetep dapet *experience* yang rapi dan nggak berantakan.

## 🛠️ Tech Stack yang Dipakai

* **HTML5:** Untuk kerangka semantik dasarnya.
* **Tailwind CSS (v4):** Buat styling utama biar kerjanya lebih cepet dan minim nulis CSS manual.
* **CSS Variables (di `base.css`):** Sengaja saya simpan warna-warna paten di sini terus dipanggil ke Tailwind pakai format kurung siku (contoh: `bg-[var(--bg-main)]`). Menurut saya ini bikin pengelolaan tema jadi lebih terpusat kalau sewaktu-waktu mau ganti palet warna.

## ✨ Highlight Fitur UI

* **Udah Responsif:** Pakai kombinasi Grid dan Flexbox. Kalau di HP bentuknya rapi memanjang ke bawah, nah pas layarnya dilebarin ke ukuran monitor, dia otomatis pecah jadi multi-kolom.
* **Horizontal Scroll di Mobile:** Khusus buat section *Features* dan *Courses*, saya akalin pakai `overflow-x-auto` ditambah `snap-mandatory`. Jadi kalau dibuka di HP, user bisa *swipe* card-nya ke samping dan nempel rapi di tengah (*snap-center*) mirip aplikasi *native*.
* **Konsistensi Visual:** Berkat CSS Variables tadi, warna background, teks, sampai border dijamin nggak ada yang belang di semua halaman.
* **Interaksi UI:** Udah saya tambahin sedikit *micro-interaction* kayak efek hover (warna berubah/redup), shadow yang muncul pas card disorot, sama transisi halus (`duration-300`) biar UI-nya kerasa lebih hidup.

## 📂 Halaman yang Udah Dibuat

Struktur pengerjaannya saya pisah jadi beberapa halaman statis:

1. **`/home.html`**: Halaman depan (*landing page*). Ada Hero banner, keunggulan platform (Why Choose EduLearn), sama preview 3 course unggulan.
2. **`/courses.html`**: Halaman list semua kelas. Saya udah nambahin mockup untuk kolom *search*, *dropdown filter*, sama pagination di bawahnya.
3. **`/about.html`**: Halaman profil, saya pakai *split layout* (gambar di kiri, teks di kanan) biar lebih enak dibaca di desktop.
4. **`/contact.html`**: Ada info kontak dan form isian. Form-nya udah dikasih efek *focus* (garis input berubah warna pas diklik) biar sesuai sama *best practice* UI/UX.

## 🎨 Daftar Warna (*Color Palette*)

* `--bg-main`: Background warna putih bersih.
* `--text-primary`: Buat judul dan teks utama (warna gelap/hitam kebiruan).
* `--text-secondary`: Buat paragraf pendukung biar mata nggak gampang capek.
* `--button-primary`: Warna biru khas DibiEdu buat tombol-tombol utama (CTA).
* `--card-main`: Warna background *off-white* khusus buat kotak/modul.

Mohon direview ya Kak, terima kasih atas masukannya!