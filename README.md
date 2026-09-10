# Laprak ProfilApp - Tugas Praktikum Bab 2 (Jetpack Compose)

- Nama: Ahmad Mustiko Wahidiyanto
- NIM: 245150207111040
- Program Studi: Teknik Informatika

## Penjelasan Singkat Kode Program

Aplikasi ini dibangun menggunakan **Jetpack Compose** untuk menampilkan kartu profil interaktif. Komponen utama yang digunakan meliputi:
1. **`ProfileScreen`**: Komposable utama yang membungkus seluruh elemen UI di dalam sebuah `Box` agar berada di tengah layar.
2. **`Card` & `Column`**: Mengelompokkan komponen profil (foto, nama, NIM, deskripsi, dan tombol) dengan tampilan latar belakang berwarna dan efek elevasi.
3. **`Image`**: Menampilkan foto profil berbentuk lingkaran menggunakan `Modifier.clip(CircleShape)`.
4. **`Text` & `Spacer`**: Menampilkan informasi teks mahasiswa dan memberikan jarak (*padding/margin*) yang rapi antar-komponen.
5. **`FollowButton`**: Komponen tombol interaktif yang memanfaatkan State Management (`remember { mutableStateOf() }`) untuk mengubah teks dari "Follow" menjadi "Unfollow" saat diklik secara real-time (*recomposition*).

## Analisis Keuntungan Jetpack Compose Dibandingkan XML Layout

1. **Pengembangan Lebih Cepat (Kurang Boilerplate)**:
   Tidak perlu membuat file layout XML terpisah dan memanggil fungsi seperti `findViewById()` atau *ViewBinding*. UI langsung ditulis menggunakan kode Kotlin.
2. **Deklaratif & Berbasis State**:
   Tampilan UI akan otomatis diperbarui (*recomposition*) ketika state data berubah, tanpa perlu mengubah properti *View* secara manual seperti pada pendekatan imperatif XML.
3. **Lebih Mudah Dikelola (Modular)**:
   UI dibangun menggunakan fungsi `@Composable` yang sangat intuitif, fleksibel, dan mudah digunakan kembali (*reusable*).
4. **Satu Bahasa Pemrograman**:
   Seluruh logika bisnis dan desain antarmuka ditulis penuh dalam bahasa Kotlin, mempercepat proses *debugging* dan pengoperasian.

---

## Tangkapan Layar (Screenshot Tampilan)

|<img width="1080" height="2400" alt="Screenshot_20260910_215511" src="https://github.com/user-attachments/assets/1a98e7e8-aee2-4018-995b-c70cecac0094" />
<img width="1080" height="2400" alt="Screenshot_20260910_215556" src="https://github.com/user-attachments/assets/8bf4a8ab-e4bb-44cb-9a5b-0f4347ba027f" />

 | <img width="2400" height="1080" alt="Screenshot_20260910_222606" src="https://github.com/user-attachments/assets/b08e6440-5644-486c-80eb-d7d1fe545b3a" />
 <img width="2400" height="1080" alt="Screenshot_20260910_222622" src="https://github.com/user-attachments/assets/d91b10d0-c267-49ab-95ed-4bbde8a7a4b6" />

|
