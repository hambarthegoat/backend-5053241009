# backend-nrp

Repo tugas mata kuliah **Pengembangan Backend Dasar**, dibuat dari template [`webdev-if-its/backend-template`](https://github.com/webdev-if-its/backend-template). Ganti judul di atas jadi nama repo kalian sendiri (`backend-nrp`, contoh: `backend-5025201012`).

## Aturan Umum

- Tugas tiap pertemuan disimpan di folder `pertemuan-XX/` pada repo ini.
- Commit message wajib menyebut level yang dicapai: `pertemuan-XX: level N selesai`.
- Deadline push: sebelum pertemuan berikutnya dimulai.
- Semua level dicek otomatis lewat `go test` — baca `pertemuan-XX/SOAL.md` tiap minggu untuk detail levelnya.

## Mengambil Pertemuan Baru Tiap Minggu

Repo ini **tidak otomatis sinkron** dengan template dosen. Begitu ada pertemuan baru, jalankan (ganti `pertemuan-02` sesuai minggu berjalan):

```bash
git fetch https://github.com/webdev-if-its/backend-template.git main
git checkout FETCH_HEAD -- pertemuan-02
```

Perintah ini **aman dijalankan kapan pun** — tidak akan menimpa folder pertemuan lain yang sudah kalian kerjakan, karena hanya mengambil folder yang disebutkan. Setelah itu, commit folder barunya seperti biasa.

Kalau dosen memperbaiki sesuatu di pertemuan yang sudah dirilis (mis. ada bug di test), biasanya cukup ambil ulang file yang diperbaiki saja, bukan seluruh folder — akan diumumkan file mana yang berubah.

---

Bagian di bawah ini **isi bertahap** sesuai level yang sedang kalian kerjakan (lihat `pertemuan-01/SOAL.md`) — heading-nya dicek otomatis, jangan diganti namanya.

## Identitas
- Nama: Muhammad Ilham Akbar
- NRP: 5053241009 
- Kelas: M

## Commit vs Push
Commit adalah dimana kita menyimpan perubahan yang telah kita buat, sedangkan push adalah dimana kita mengirimkan commit ke remote repository.

## Reproducibility
Reproducibility berarti kode menghasilkan output yang sama di lingkungan yang berbeda. Sebagai contoh, jika anggota tim menjalankan program ini dengan versi Go yang berbeda (misal go1.21 vs go1.23), biasanya tidak masalah untuk kode sederhana seperti ini karena CetakInfo sendiri mencetak runtime.Version() sehingga perbedaan itu terlihat jelas. Tapi ini bisa jadi masalah nyata kalau kode memakai fitur bahasa atau standard library yang baru ditambahkan di versi tertentu yang memakai Go versi lebih lama akan gagal compile, atau kalau ada perubahan behavior antar versi (misal urutan map berubah, atau fungsi deprecated dihapus), hasil program bisa berbeda meski source code-nya sama.

## Catatan Merge Conflict
Catatan merge conflict adalah catatan yang muncul ketika terjadi konflik saat melakukan merge, yaitu ketika ada perubahan yang berbeda antara branch yang sedang kita kerjakan dan branch yang akan di-merge. Di sini, branch main dan branch fitur-sapaan keduanya melakukan commit yang mengubah 1 line yagn sama dengan hasil berbeda, menyebabkan adanya coflict yang harus di resolve secara manual, disini saya memilih accept both changes

## Kenapa .gitignore Penting
.gitignore adalah file yang digunakan untuk menentukan file mana yang akan di-ignore oleh Git, yaitu file yang tidak akan dimasukkan ke dalam repository. Ini penting untuk menjaga kebersihan repository dan menghindari file yang tidak perlu di-commit.

## Refleksi
Tidak ada soal yang membingungkan, semua soal sudah jelas dan straightforward.  