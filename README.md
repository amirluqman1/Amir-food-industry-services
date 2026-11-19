# Amir Food Industry Services

Rangka website satu fail untuk A.F.I.S. Kandungan syarikat (hero, tentang kami, projek, servis, statistik, footer dan borang) sudah diisi. Yang masih kosong: gambar hero (`IMAGES.heroBase` dan `IMAGES.heroReveal`).

Borang "Dapatkan Sebut Harga" membuka WhatsApp dengan mesej siap ditaip ke nombor dalam `const WHATSAPP`. Angka statistik ada dalam `COUNT_TARGETS`.

## Kandungan yang boleh diisi kemudian

Buka `index.html` dan cari `const CONTENT` pada awal `<script type="module">`.

- `brand.*`: nama dan watermark.
- `nav.*`, `header.*`, `menu.*`: navigasi dan ruang maklumat header.
- `hero.*`, `carousel.*`: tajuk utama, butang, kad dan rakan niaga.
- `about.*`, `band.*`: pengenalan dan empat pil.
- `portfolio.*`: empat kad, tajuk, penerangan dan tag.
- `services.*`: empat baris perkhidmatan.
- `stats.*`: tajuk, label dan akhiran statistik. Isi angka sebenar dalam `COUNT_TARGETS`.
- `footer.*`, `request.*`: footer dan borang modal.

Nilai yang belum diputuskan kekal sebagai `""`. Ruang perkataan kosong mengekalkan pembalutan baris dan tinggi layout. Apabila sesuatu nilai diisi, teks menggantikan ruang kosongnya. Kandungan yang lebih panjang akan mengalir secara semula jadi mengikut layout responsif.

Isi URL gambar hero dalam `IMAGES.heroBase` dan `IMAGES.heroReveal`. Logo asal telah dibenam sebagai data URI dalam `IMAGES.brandMark` supaya laman kekal satu fail HTML. `heroAlt` untuk penerangan aksesibiliti gambar utama. Tiada gambar dimuat turun selagi URL kosong; kanvas berus hanya berjalan apabila kedua-dua gambar hero diisi. Jangan letak `src=""` pada imej.

Label pembaca skrin dan pautan langkau kandungan kekal untuk aksesibiliti.

## GitHub Pages

Laman tidak memerlukan pemasangan atau build. Dalam **Settings → Pages**, pilih **Deploy from a branch**, cawangan **main** dan folder **/(root)**, kemudian simpan. `index.html` mesti kekal di root repo. Fail `.nojekyll` mengekalkan penerbitan HTML statik.

## Ikon dan pratonton pautan

- `favicon-32.png`: ikon tab pelayar. `apple-touch-icon.png`: ikon bila laman disimpan ke skrin utama iPhone.
- `og-image.jpg` (1200×630): gambar yang keluar bila pautan dikongsi di WhatsApp, Facebook dan lain-lain. Tag `og:*` dalam `<head>` guna URL penuh laman; kalau alamat laman bertukar (contoh: domain sendiri), kemas kini URL tersebut.

## Dokumen pendaftaran (kemas kini berkala)

- **TCC (Sijil Pematuhan Cukai)** diperbaharui setiap tahun. Sijil semasa luput 31/12/2026. Bila TCC baru dapat, semak ayat dalam `services.paragraph.4` masih tepat.
- **MOF** sah hingga 14/10/2029. Tahun dalam `services.paragraph.4` ("hingga 2029") perlu dikemas kini bila diperbaharui.
- Jangan letak dokumen asal (SSM, MOF, TCC) dalam repo ini: repo awam dan dokumen tersebut mengandungi maklumat peribadi.

## Gambar

- `img/hero-bufet.jpg`: gambar hero (dipasang dalam `IMAGES.heroBase`). Lapisan gelap atas gambar diatur dalam CSS bertanda "Gambar hero".
- `img/hero-vip.jpg`: versi "VIP" yang terdedah bila mouse digerakkan atas hero (efek berus, `IMAGES.heroReveal`). Dijana AI, kemudian dijajarkan dengan `hero-bufet.jpg`; tepi atas dan bawah kekal gambar asal. Efek ini hanya berfungsi dengan mouse (desktop).
- `img/kantin-mfs.jpg`: latar kad projek "MFS Technology" (kantin kilang).
- `img/kantin-smk.jpg`: latar kad projek "SMK Seri Bemban". Muka pelajar yang jelas dikaburkan satu per satu (bawah umur); jangan ganti dengan versi asal tanpa kebenaran sekolah.
- `img/permulaan-gerai.jpg`: gambar gerai No. 26 (permulaan A.F.I.S; gerai di sebelah kanan gambar. Kedai kiri, Desa Food No. 27, bukan milik A.F.I.S) dalam bahagian Tentang Kami.
- `img/event-utem.jpg`: latar kad projek "UTeM Melaka" (event sup daging 7,000 pax).
- `img/makanan-packing.jpg`: latar kad projek "Makanan Packing".
- Gambar dikecilkan (~1200px) dan data EXIF (termasuk lokasi GPS) dibuang sebelum dimasukkan. Buat perkara sama untuk gambar baru.
