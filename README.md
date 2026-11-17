# Amir Food Industry Services

Rangka website satu fail, berdasarkan susunan, font Onest, grid rem adaptif, spacing, warna dan animasi laman rujukan. Semua kandungan teks, logo, gambar, pautan sosial dan angka statistik sengaja dibiarkan kosong. Tiada teks contoh atau gambar stok ditambah.

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

Semua nilai bermula sebagai `""`. Ruang perkataan kosong mengekalkan pembalutan baris dan tinggi layout. Apabila sesuatu nilai diisi, teks menggantikan ruang kosongnya. Kandungan yang lebih panjang akan mengalir secara semula jadi mengikut layout responsif.

Isi URL gambar dalam `IMAGES.heroBase`, `IMAGES.heroReveal` dan `IMAGES.brandMark`. `heroAlt` untuk penerangan aksesibiliti gambar utama. Tiada gambar dimuat turun selagi URL kosong; kanvas berus hanya berjalan apabila kedua-dua gambar hero diisi. Jangan letak `src=""` pada imej.

Label pembaca skrin dan pautan langkau kandungan kekal untuk aksesibiliti. Nombor loader 000–100 dan ikon kawalan ialah sebahagian interaksi, bukan kandungan syarikat. Borang masih simulasi sahaja: tiada permintaan dihantar ke pelayan.

## GitHub Pages

Laman tidak memerlukan pemasangan atau build. Dalam **Settings → Pages**, pilih **Deploy from a branch**, cawangan **main** dan folder **/(root)**, kemudian simpan. `index.html` mesti kekal di root repo. Fail `.nojekyll` mengekalkan penerbitan HTML statik.
