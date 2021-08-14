### Perintah

Awali perintah dengan `/`, `!`, atau `#`.

Perintah | Rincian | Status | Superuser | Admin Global | Admin Grup | Pengguna biasa
--- | --- | --- | --- | --- | --- | --- |
`/hammer` | `[menggunakan reply/username/id]`  _Ban_ secara global | ✅ | ✅ | ✅ | ❌ | ❌
`/unhammer` | `[menggunakan reply/username/id]`  _Unban_ secara global | ✅ | ✅ | ✅ | ❌ | ❌
`/leave` | Bot meninggalkan grup | ✅ | ✅ | ❌ | ❌ | ❌
`/promote` | `[menggunakan reply/username/id]`  Angkat _user_ sebagai admin global | ✅ | ✅ | ❌ | ❌ | ❌
`/demote` | `[menggunakan reply/username/id]`  Turunkan _user_ dari jabatan admin global | ✅ | ✅ | ❌ | ❌ | ❌
`/banlist` | Kirim berkas txt ke kanal pencatat, berisi nama _user_ yang di-_ban_ secara global | ✅ | ✅ | ✅ | ❌ | ❌
`/admins` | Tampilkan daftar admin-admin grup | ✅ | ✅ | ✅ | ✅ | ✅
`/globaladmins` | Tampilkan daftar admin-admin global | ✅ | ✅ | ✅ | ✅ | ✅
`/kick` | Keluarkan _user_ dari grup (dapat bergabung kembali) | ✅ | ❌ | ❌ | ✅ | ❌
`/ban` | _Ban user_ dari grup | ✅ | ❌ | ❌ | ✅ | ❌
`/start` or `/help` | Tampilkan bantuan dalam beragam bahasa | ✅ | ✅ | ✅ | ✅ | ✅

#
Anda perlu Node.js versi > 4, untuk mengunduh _dependencies_ dan menjalankan bot ini.  
Untuk pengguna Windows, cukup klik [berkas ini](https://nodejs.org/dist/v7.4.0/node-v7.4.0-x64.msi) untuk memasangnya.  
Untuk pengguna Unix, gunakan cara sesuai distro atau rujuk [laman ini](https://nodejs.org/en/download/).

```bash
# Pastikan Anda telah memasang paket Node.JS! 
$ node -v

# Clone repo
$ git clone https://github.com/rizaumami/TGramIndoBot.git
$ cd TGramIndoBot
# Pastikan semua baris dalam data/config.json diisi!

# Masuk ke dalam akun Openshift web console Anda
# Buat sebuah app
# Pilih Node.js [Latest]
# 
# jalankan app
# Tambahkan  cartridge > Install your own cartridge
# Masukkan laman ini => https://raw.githubusercontent.com/icflorescu/openshift-cartridge-mongodb/master/metadata/manifest.yml
# Tambahkan ssh keys Anda ke Openshift dan pastikan kunci tersebut ada di $HOME/.ssh
# Salin laman git yang berada di kolom kiri laman web console

$ git remote add openshift [LAMAN REMOTE GIT, SALIN DARI LANGKAH DI ATAS]
$ git push openshift master --force
```

## Lisensi

Dirilis dibawah lisensi AGPL-v3.0, lihat berkas [LICENSE](https://github.com/lanzvian/LanzBot-2/blob/master/LICENSE).
