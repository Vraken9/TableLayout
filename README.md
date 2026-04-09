## Ringkasan Proyek

Realisasi pendirian lembar etalase kasir pada tabulasi harga dirangkai utuh
berpedoman `<TableLayout>` di sistem. Selaput bilik data tidak didokrak sejajar
horisontal, melainkan tersusun dari injeksi rangka pemenggal lantai baja yang
dinamakan `<TableRow>`. Seutas pilar yang hinggap di bahu bingkai pinggiran barisnya
akan bersinkronisasi rapi didaulat menjadi tiang kolom indeksnya masing-masing.
Untuk memerangi bahaya celah sunyi antar layar gawai, dititipkan atribut mutlak
berupa `android:stretchColumns="1"`, mengakibatkan bilik penjabaran spesies bunganya
memuai menegang secara dramatis menginvasi batas kekosongan yang merugikan.

## Dokumentasi Teknis

### 1. Penjelasan File Resource Pendukung

Sengketa pemisah tabel hambar konvensional dibantu jajaran gurat hiasan kanvas res
memukau buatan batin programmer dari tabung gambar `table_border`, `header_bg`.

-   **Fungsinya:** Kode arsip ini merias sentuhan pemanis cangkang tabel. Contohnya,
    tabel yang dibalut `table_border` dirapal menduplikasi gaya balok sel surya
    dengan ketebalan benang tepian tegas, menumbuhkan rona gagah kaku namun beradab.
    Atap penamaan (*header row*) dicat hitam membaur demi mempertegas indeks atasan.
-   **Mengapa dipisah?:** Pemahatan ornamen bingkai tabel merenggut korban untaian
    sandi pembentukan wujud asimetris panjang dari balok format `Shape/Stroke/Solid`.
    Alih-alih mengotori dokumen letak (*layout*) suci dengan gerombolan cat desain 
    radius kotak, menyingkirkannya ke arsip `drawable` menjaga silsilah peninggalan
    dokumentasi murni bersih perihal arsitektur pembagian bilah tulang layar semata.

### 2. Penjelasan Logika Layout Utama (`activity_main.xml`)

Keanggunan **TableLayout** menyempurnakan kegagapan mesin konvensional saat dimintai
tolong mensinkronkan barisan teks beda bobot karakter menjadi satu patokan penggaris.

-   **Tatanan Roda Traktor `<TableRow>`**: Jangan bayangkan *layout_width* berguna di 
    lembar barisan sel ini. TableRow tak mempedulikan teriakan lebar komponennya.
    Pemrograman bersikap diktator menjulurkan baris renggang menjejalkan ke batas 
    akhir layar. Pilar biliknya murni mengadopsi tatanan muasa selebar anak perut 
    konten bawaan pembatasannya murni (`WRAP_CONTENT`).
-   **Sinkronisasi Baris Gaib**: Kekuatan gaibnya merajut bila baris kesepian atas
    bertuliskan dua huruf singkat, lalu balok kesepuluh meledak kalimat "Daging Bunga 
    Tercabik"; seluruh jejak menjejak lajur kolom mengayun memuja tiang perataan 
    ukuran si komponen raksasa. Mencegah runtuhnya barisan bagai rumah kartu rontok.
-   **Tali Pemelaran Otot (`stretchColumns="1"`)**: Demi menutup luka jarak layar yang 
    lebar bervariasi, ikatan pilar tipe 1 (Terhitung lompatan awal bernilai ke nol) 
    yakni wadah 'Jenis Kelamin Bunga', diperkosa memelar ke samping menutup tirai
    ruang tak bertuan. Mencegah tampilan selokan kosong menakutkan mencuat tajam.

### 3. Alur Visual

Segenap layar dilenggangkan berdansa bak instrumen pendaftaran kasir jadul nan apik:

1.  **Benteng Langit Atasan Bintang (Header Row)**: Segerombolan huruf terbit mulus
    dipangkas tebal bertinta putih bersimpuh dalam pakaian jas legam. Kolom No, Nama, 
    hingga Nominal menengadah congkak sebagai gerbang kompas petunjuk pembagian tabel.
2.  **Sembilan Celurit Pisau Pembelah (Divider View)**: Tanpa manipulasi ornamen ruit, 
    digunakan jurus *View* telanjang berlapis kelengangan ukuran tubuh tipis segaris, 
    `1dp` pisau silet melukai daging layar mewujud pemisah pagar pembatas antar sel.
3.  **Aksi Pasar Bursa (Row Item Data)**: Membujur tumpukan demi tumpukan entri buku
    perdagangan mawar menjabat erat mahar nilai harganya di ujung sela terpisah. Agar 
    tampak berjas intelek, kotak pembungkus pilar spesie dijejalkan persekutuan menara
    *TextView* vertikal menumpuk rona tebal dan tipis dalam bingkai yang tetap stabil
    memotong barisan rapi tanpa mengungkit ukuran tinggi seiringan baris.
4.  Lantai pambaling pun meremuk diakhiri ketukan sabda kelip pesan pelindung ("Harga
    tak terprediksi bagai ombak"). Ditutup bungkusan pelarut usapan `ScrollView`
    manakala si empunya kasir menggila memborong ratusan peranti pembukuan tambahan!
