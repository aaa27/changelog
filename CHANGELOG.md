# Changelog
Aplikasi  Manajemen  Sertifikat  Elektronik  (AMS)  adalah  aplikasi  yang dikembangankan  dan  dikelola  Balai  Sertifikasi  Elektronik  (BSrE)  untuk melakukan  proses  pendaftaran,  pembaruan,  pencabutan  dan  monitoring sertifikat elektronik milik BSrE. Pada aplikasi AMSterdapat beberapa roles, diantara lain, Registration Authority(RA),  Verifikator dan Pengguna.

Dengan   AMS   ini,   pengguna   dapat   melakukan   manajemen   sertifikat elektronik miliknya. Mulai dari pengajuan pendaftaran sertifikat elektronik, pembaruan sertifikat elektronik, pengajuan pencabutan sertifikat elektronik, melakukan resetpassphrasesertifikat  elektronik  dan  memonitor  proses sertifikat elektronik miliknya secara mandiri

Semua perubahan penting pada aplikasi ini akan di dokumentasikan dalam file ini. File ini dibuat merujuk pada [standard-version](https://github.com/conventional-changelog/standard-version)

## v4.8.2
#### Pembaruan 
- Menerima berbagai macam format CSV
- Semua inputan data dari CSV diubah menjadi huruf kecil

## v4.8.1
#### Pembaruan 
- Verifkator dan RA_Instansi bisa mengubah data pengguna

## v4.8.0
#### Pembaruan 
- Perbaikan pada fitur ubah email , nik, dan atribut di AMS-Core tidak secara otomatis memperbarui data di Keycloak
- Penerbitan ulang dan pembaruan SrE dengan KYC
- Penyesuaian pilihan alasan pencabutan SrE
- Alasan penolakan aktivasi akun pada menu di AMS dan pada email pemberitahuan ke pengguna
- Filter pencarian berdasarkan status akun dan status sertifikat elektronik
- Pembatasan karakter untuk isian Nama Lengkap pada fungsi Tambah (Satu) Pengguna (ADMIN)
- Perbaikan pada fungsi penambahan pengguna menggunakan CSV
- penerbitan ulang dan pembaruan SrE tidak dengan KYC (ADMIN)

#### Penghapusan 
- Toggle enable/disable messaging WhatsApp
- Menghilangkan field nomor HP
- Penonaktifan akun pengguna dihilangkan

## v4.7.1
#### Penambahan 
- Verifikator instansi tidak dapat melakukan unduh laporan analitik pada tahun sebelumnya
- AMS memfasilitasi data analitik pada satu tahun sebelumnya sampai dengan tahun berjalan

## v4.7.0
#### Penambahan 
- Menambahkan notifikasi “Silakan buka Google Auth Anda untuk mendapatkan Kode OTP”.
- Menghapus opsi pilihan FreeOTP.
- Menampilkan halaman Manage OTP di AMS. Menampilkan Password, Auth, Session, Sign Out. 

#### Pembaruan 
- Menambahkan notifikasi di Aplikasi dan Email informasi akun.
```
- Non-ASN: Aktivasi Berhasil. Silakan menghubungi verifikator pada Unit IT Instansi untuk Verifikasi akun.
- ASN: Aktivasi Berhasil. Silakan mengecek email untuk set passphrase.
- Apabila ditolak, alasan penolakan ditampilkan di email pemberitahuan.
- Push notifikasi ke Email atau Whatsapp Verifikator yang berisi
- notifikasi terkait ada akun pengguna yang menunggu proses Verifikasi sebagai reminder. 
```
- Penamaan subject email sesuai dengan aktivitas user, seperti set passphrase penerbitan sertifikat elektronik, reset passphrase, pembaruan sertifikat elektronik. 
- Menampilkan kembali fitur unggah SR Verifikator dan Verifikator menyetujui perjanjian verifikator
- Aktifkan kembali restricted email dinas dan pengecekan email dinas, untuk pendaftaran satu pengguna, beberapa pengguna, dan csv.
- Menonaktifkan Case Sensitive saat input email. 
- Notifikasi Error saat set passphrase menjadi, “Gagal set passphrase, mohon mencoba kembali beberapa saat”

#### Perbaikan 
- Muncul pop-up alur bagaimana mendapatkan segel (hanya untuk verifikator), ketika belum ditambahkan produk segel pada instansi
- Menampilkan data pemilik segel pada menu Pemilik Segel di AMS.
- Notifikasi error/gagal saat ubah data disesuaikan dengan kesalahan/kekeliruan yang dibuat (tidak seluruh notif “Silahkan isi form berikut ya”) 

## v4.6.2
#### Perbaikan
- Fitur kirim email ke beberapa pengguna
- Penyesuaiaan produk TLS/SSL

## v4.6.1
#### Pembaruan 
- Membatasi opsi periode unduh laporan PSrE dengan menonaktifkan bulan berjalan
- Mengganti tanda desimal nilai transaksi TTE dari tanda titik "." menjadi tanda koma ","

## v4.6.0
#### Penambahan 
- Tanggal Expired PKS (Akun Verifikator);
- Jumlah Aplikasi Terintegrasi (Akun Verifikator);
- Jumlah Pengguna (Akun Admin, RA, Verifikator);
- Jumlah Sertifikat Issued, Revoke (Akun Admin, RA, Verifikator);
- Jumlah transaksi TTE (Akun Admin, RA, Verifikator);
- Grafik Pengguna per waktu (Akun Admin, RA, Verifikator);
- Grafik Sertifikat per waktu (Akun Admin, RA, Verifikator);
- Grafik TTE per waktu (Akun Admin, RA, Verifikator);
- Download Excel Rekapitulasi Pengguna (nama, instansi, status pengguna, status sertifikat, jumlah TTE);
- Download laporan bulanan (sesual dengan contoh laporan ke kominfo);
- Grafik Analisa Prediktif Pertumbuhan TTE instansi dalam satu tahun kedepan;
- Grafik Analisa Prediktif Pertumbuhan Pengguna Instansi dalam satu tahun kedepan;
- Data analitik filter per individu by NIK atau Email;
- Grafik TTE per waktu.

#### Pembaruan 
- Menampilkan kembali fitur unggah SR Verifikator dan Verifikator menyetujui perjanjian verifikator 

#### Perbaikan 
- Error notifikasi

## v4.5.0
**Pembaruan**
- Alasan pencabutan sertifikat elektronik
- Tombol pembaruan sertifikat elektronik akan aktif ketika masa valid sertifikat elektronik kurang dari samadengan 30 Hari

**Perbaikan**
- Pengecekan data pengguna ketika data _profile_ pengguna kosong setelag berhasil _login_
- Security issue 5.1.2
- Security issue 5.1.3

## v4.4.0
#### Penambahan 
- Filter "produk" pada setiap menu verifikasi (penerbitan, pembaruan,
pencabutan) dan pada Menu "Pengguna"

#### Pembaruan
- Label Field Common Name menjadi Nama Organisasi

#### Perbaikan 
- Menghapus Field Unit Ogranisasi 
- Label pada form konfirmasi ketika "permohonan pembaruan"
- Menghapus fitur "ubah
passphrase" dan "reset passphrase" pada tombol "Aksi" pada sertifikat

## v4.3.1
#### Pembaruan Fitur
- Peningkatan performa aplikasi pada saat proses persetujuan permohonan

#### Penghapusan Fitur
- Menghilangkan sementara "dashboard verifikator"

## v4.3.0
#### Penambahan Fitur
- Notifikasi informasi kepada RA saat melakukan tambah verifikator sudah lebih dari 3 orang
- Cek Surat Rekomendasi yang diupload di AMS saat pendaftaran Verifikator, SSL, Segel dll harus dokumen ber TTE dan bisa di verifikasi

#### Pembaruan Fitur
- Verifikasi Pengguna oleh Verifikator jika NIK di WHITELIST atau Kuota Pengecekkan Dukcapil Habis
- Perubahan Notifikasi NIK Tidak Terverifikasi saat Pengecekkan Nama dan NIK

#### Penghapusan Fitur
- Penghapusan opsi “Buat Passphrase” dan “Aktivasi Verifikator” di halaman Overview
- Penghapusan list “Surat Rekomendasi” di halaman Jenis Permohonan

## v4.2.0
#### Penambahan Fitur
- Fitur sync akun oleh Role ADMIN

#### Pembaruan Fitur
- Menampilkan foto profile pengguna
- Menampilkan foto selfie pengguna ketika proses verifikasi oleh verifikator
- Menambahkan waktu idle maksimal (12 Jam), maka aplikasi akan logout secara otomatis

#### Penghapusan Fitur
- Menghapus beberapa pengriman pranala ulang ke pengguna oleh verifikator
- Menghilangkan status (aktif/tidak) pengguna
 
#### Perbaikan
- Auto sync ketika login pertama kali ke AMS versi 3 atau versi di atasnya
- Penghapusan data dummy yang tertinggal pada beberapa vue component

## v4.1.1
#### Pembaruan Fitur
- Perubahan format waktu dan tanggal
- Update form (csv) pendaftaran pengguna
- Penambahan role Kordinator RA
- Mengaktifkan fitur eSeal versi Beta
- Penyesuaian tabel Verifikator dan RA
- Pengecekan Email Dinas
- Menghilangkan data dukung pada proses permohonan ESign
- Menambahkan akses ke BSrE Client Kit

#### Perbaikan
- Ubah data pengguna oleh verifikator instansi 
- Auto Approval pada proses permohonan ESign
- Perubahan Status pengguna
- Penambahan Verifikator dan RA

## BSRE CA v4.0.1
#### Penambahan Fitur
- Pengecekan data ASN ke BKN pada saat proses aktivasi pengguna
- Pengecekan data kependudukan ke DUKCAPIL
- Informasi akan hadir produk SSL
- Informasi akan hadir produk eSEAL
- Peningkatan performa

#### Pembaruan Fitur
- Pembaruan layanan Segel Elektronik
- Pembaruan proses bisnis pendaftaran pengguna
- Pembaruan proses bisnis penerbitan sertifikat elektronik
- Pembaruan proses bisnis pengajuan sebagai verifikator instansi

## BSRE CA v4.0.0 (04-11-2022)
#### Penambahan Fitur
- Pengecekan data ASN ke BKN pada saat proses aktivasi pengguna
- Penerbitan sertifikat elektronik SSL
- Penerbitan sertifikat elektronik Extended Validation SSL
- Penerbitan sertifikat elektronik SSL Client

#### Pembaruan Fitur
- Pembaruan layanan Segel Elektronik
- Pembaruan proses bisnis pendaftaran pengguna
- Pembaruan proses bisnis penerbitan sertifikat elektronik
- Pembaruan proses bisnis pengajuan sebagai verifikator instansi

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


