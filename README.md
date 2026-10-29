# KIRI — Character Status Manager (v2)

Aplikasi statis HTML untuk mencatat karakter novel Kiri Finslein dan menyalin status dalam format konsisten.

## Deploy via GitHub + Vercel

1. Buat repository baru di GitHub.
2. Unggah `index.html` dan `README.md` ke **root** repository (bukan di dalam subfolder).
3. Masuk ke Vercel → **Add New → Project** → impor repository GitHub tersebut.
4. Pilih framework **Other** (aplikasi HTML statis), tanpa build command. Deploy.
5. Buka alamat situs yang diberikan Vercel.

## Penting: penyimpanan data

- Data tersimpan dalam **localStorage browser pada perangkat dan alamat situs tersebut**. Vercel/GitHub **tidak menyimpan database karakter**.
- Data **tidak otomatis sinkron antar perangkat**, bahkan jika masuk ke alamat Vercel yang sama.
- Gunakan **Backup JSON** rutin dan **Pulihkan Backup** ketika berpindah perangkat/browser.
- Perubahan domain Vercel atau menghapus data browser bisa membuat data lama tidak muncul. Simpan file backup sebelum melakukannya.
- Undo hanya menyimpan maksimal 50 perubahan dalam sesi terbuka, bukan histori permanen.

## Fitur v2

- Database karakter dan editor Core/Rank, Aspect, Attribute, Skill.
- Level Skill hanya untuk protagonis Kiri.
- Tampilan status catatan penulis vs inspeksi Kiri (Skill karakter lain disembunyikan pada mode inspeksi).
- Penanda manual ketika informasi target terlalu kuat untuk diperiksa.
- Undo terbatas, validasi impor dan nama Skill, ekspor/impor JSON, pemeriksaan penyimpanan.

## Batasan

- Belum ada akun, cloud sync, atau backend.
- Belum ada modul Farming, Harvest Storage, maupun riwayat perkembangan per chapter.
