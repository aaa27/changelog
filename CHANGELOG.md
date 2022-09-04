# Changelog
Aplikasi  Manajemen  Sertifikat  Elektronik  (AMS)  adalah  aplikasi  yang dikembangankan  dan  dikelola  Balai  Sertifikasi  Elektronik  (BSrE)  untuk melakukan  proses  pendaftaran,  pembaruan,  pencabutan  dan  monitoring sertifikat elektronik milik BSrE. Pada aplikasi AMSterdapat beberapa roles, diantara lain, Registration Authority(RA),  Verifikator dan Pengguna.

Dengan   AMS   ini,   pengguna   dapat   melakukan   manajemen   sertifikat elektronik miliknya. Mulai dari pengajuan pendaftaran sertifikat elektronik, pembaruan sertifikat elektronik, pengajuan pencabutan sertifikat elektronik, melakukan resetpassphrasesertifikat  elektronik  dan  memonitor  proses sertifikat elektronik miliknya secara mandiri

Semua perubahan penting pada aplikasi ini akan di dokumentasikan dalam file ini. File ini dibuat merujuk pada [standard-version](https://github.com/conventional-changelog/standard-version)

## v3.0.0
Dirilis pada tanggal : 31-06-2022
### Added
- manajemen akun pengguna terpusat
- login dengan 2FA 
- terintegrasi dengan sistem data kependudukan
- penambahan fitur segel elektronik (beta)

### Update
- peningkatan performa aplikasi

## v2.3.1
Dirilis pada tanggal : 04-03-2022
### Update
- perbaikan bug pendaftaran pengguna menggunakan CSV file
- penyesuaian waktu sesuai dengan GMT+7
- integrasi pendaftaran dengan data wilayah

## v2.3.0
Dirilis pada tanggal : 06-12-2021
### Added
- integrasi dengan service wilayah

### Update
- Menu penerbitan Sertifikat elektronik

### Delete
- live chat BSrE
- Menu penerbitan PKCS#12
- login method with keycloak 

## v2.2.0
Dirilis pada tanggal : 13-08-2021
### Added
- login method with keycloak 

## v2.1.9
Dirilis pada tanggal : 05-08-2021
### Added
- 'details' button to display more complete user information

### Changed
- sorting by date in table

## v2.1.8
Dirilis pada tanggal : 03-08-2021
### Fixed
- Information on list of users whose electronic certificates are about to expire

## v2.1.7
Dirilis pada tanggal : 31-07-2021
### Fixed
- Approval modal

### Removed
- User activity list

## v2.1.6
Dirilis pada tanggal : 30-07-2021
### Fixed
- Filter by segel owner
- Notification when the session time is about to end
- Login Notification
- Document preview

### Update
- Continue the process of exporting data if the session time is up
- New look at process user activation
- Upload supporting documents on the menu management ra and verifier

### Added
- Changloge
- Data verification officer information 
- List of users whose electronic certificates are about to expire
- User data history list
- User activity list

### Changed
- Validation of user activation form
- Disable the change user data tab if the user status is new

## v2.1.5
Dirilis pada tanggal : 18-07-2021
### Fixed
- Delete data pengguna ada local storage browser setelah selesai export data
- HTTP Status 5xx

## v2.1.4
Dirilis pada tanggal : 17-07-2021
### Changed
- Synchronous Request pada proses export data pengguna, dan proses berjalan di background aplikasi

### Fixed
- Revoke sertifikat pengguna

## v2.1.3
Dirilis pada tanggal : 16-07-2021
### Added
- `Menangguhkan / Mengaktifkan` sertifikat elektronik
- Filter berdasarkan status sertifikat elektronik
- Export data verifikator

### Changed
- Parallel Request pada proses export data pengguna
- Pembatasan informasi yang diberikan pada tabel hasil export pengguna / verifikator

## Fixed
- `Menangguhkan / Mengaktifkan` sertifikat elektronik dan pengguna
- Urutan Tanggal pada label grafik
- Responsive dropdown aksi pada table daftar sertifikat elektronik
- Typo button `Reload`

## v2.1.2
Dirilis pada tanggal : 11-07-2021
### Changed
- Hanya Admin dan RA BSrE yang dapat melakukan filter `Include / Exclude` Instansi

### Fixed
- Tombol loading pada table pengguna saat proses mencari data
- Filter pada table `Manajemen RA`
- Logout secara otomatis jika sesi login sudah habis

## v2.1.1
Dirilis pada tanggal : 10-07-2021
### Added
- Fiter dan Sorting pada tabel daftar pengguna di menu `Tambah Beberapa Pengguna`
- Form `Organisasi` pada menu `Tambah beberapa pengguna dari file csv`
- Component `Surat Rekomendasi`
- Informasi status `SEGEL`
- `Reload` data pada tabel
- Filter `Include / Exclude` Instansi

### Fixed
- Notifikasi pada saat aktivasi akun
- `Menangguhkan / Mengaktifkan` kembali instansi
- Dropzone pada menu tambah beberapa pengguna
- Notifikasi setelah proses tambah beberapa pengguna
- Form pilih Surat Rekomendasi
- Notifikasi setalah melakukan `Menangguhkan / Mengaktifkan`
- Filter pada setiap tabel
- Filter pada menu `Manajemen RA`

### Changed
- Notifikasi saat proses `KYC` gagal
- Format csv File untuk tambah pengguna
- Notiifikasi saat proses `Aktivasi Akun`
- Pembatasan, maksimal 100 data saat tambah beberapa pengguna
- Form pilih surat rekomendasi di setiap permohonan
- Menampilkan tombol `Menangguhkan / Mengaktifkan` pada table pengguna
- Pembatasan unggah file maksimal 1 Mb
- Form `Reason` ketika proses `Menangguhkan / Mengaktifkan`

## v2.1.0
Dirilis pada tanggal : 29-06-2021
### Added
- ADMIN dapat `Menangguhkan / Mengaktifkan` kembali pengguna
- ADMIN dapat `Menangguhkan / Mengaktifkan` kembali instansi
- Integrasi `Live Chat` Call Center BSrE.
- `Petunjuk Teknis` penggunaan aplikasi AMS 2.0
- Integrasi `KYC` pada proses aktivasi akun
- Tambah Beberapa Pengguna
- Tambah beberapa pengguna dari file csv

### Changed
- Form Organisasi Unit menjadi Alpha Numeric
- Tidak ada maksimum panjang karakter pada form Organisasi Unit


