# CAHAYA-MITRA-JAYA-MANDIRI
Bidang Usaha: Kontraktor Bangunan, Renovasi, &amp; Distributor / Supplier Material Pengamanan (Pagar BRC, Kawat Silet, Kawat Duri)
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CAHAYA MITRA JAYA MANDIRI - Jasa Konstruksi & Pagar BRC</title>
    <!-- Google Fonts & FontAwesome -->
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700;800&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary-purple: #4a154b;
            --light-purple: #7c227e;
            --accent-red: #d32f2f;
            --accent-yellow: #ffb300;
            --dark-bg: #1a1a1a;
            --light-bg: #f9f9f9;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Poppins', sans-serif;
            scroll-behavior: smooth;
        }

        body {
            background-color: var(--light-bg);
            color: #333;
        }

        /* Header & Navbar */
        header {
            background: linear-gradient(135deg, var(--primary-purple), var(--light-purple));
            color: white;
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 4px 10px rgba(0,0,0,0.3);
            border-bottom: 4px solid var(--accent-yellow);
        }

        .navbar {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 20px;
        }

        .logo {
            font-size: 1.2rem;
            font-weight: 800;
            color: var(--accent-yellow);
            display: flex;
            align-items: center;
            gap: 10px;
            text-shadow: 1px 1px 2px rgba(0,0,0,0.5);
        }

        .nav-links {
            display: flex;
            gap: 20px;
            list-style: none;
        }

        .nav-links a {
            color: white;
            text-decoration: none;
            font-weight: 600;
            transition: 0.3s;
            font-size: 0.95rem;
        }

        .nav-links a:hover {
            color: var(--accent-yellow);
        }

        /* Hero Banner Utama */
        .hero-banner {
            background: linear-gradient(rgba(74, 21, 75, 0.85), rgba(211, 47, 47, 0.85)), url('https://images.unsplash.com/photo-1541888946425-d0fbb18f244c?auto=format&fit=crop&w=1200&q=80');
            background-size: cover;
            background-position: center;
            color: white;
            text-align: center;
            padding: 60px 20px;
            border-bottom: 5px solid var(--accent-yellow);
        }

        .hero-banner h1 {
            font-size: 2.2rem;
            font-weight: 800;
            margin-bottom: 10px;
            color: var(--accent-yellow);
            text-shadow: 2px 2px 4px rgba(0,0,0,0.6);
        }

        .hero-banner p {
            font-size: 1.1rem;
            max-width: 800px;
            margin: 0 auto 20px auto;
        }

        /* Iklan Gudang & Foto Kiriman */
        .ad-section {
            max-width: 1100px;
            margin: -30px auto 30px auto;
            padding: 0 20px;
            position: relative;
            z-index: 10;
        }

        .ad-card {
            background: white;
            border-radius: 12px;
            box-shadow: 0 10px 25px rgba(0,0,0,0.2);
            overflow: hidden;
            border: 3px solid var(--accent-yellow);
            display: grid;
            grid-template-columns: 1fr 1fr;
            align-items: center;
        }

        @media(max-width: 768px) {
            .ad-card {
                grid-template-columns: 1fr;
            }
            .nav-links {
                display: none;
            }
        }

        .ad-image img {
            width: 100%;
            height: 350px;
            object-fit: cover;
            display: block;
        }

        .ad-content {
            padding: 30px;
            background: #fff;
        }

        .badge-promo {
            background: var(--accent-red);
            color: white;
            padding: 5px 12px;
            font-size: 0.85rem;
            font-weight: 700;
            border-radius: 20px;
            display: inline-block;
            margin-bottom: 15px;
            text-transform: uppercase;
        }

        .ad-content h2 {
            color: var(--primary-purple);
            font-size: 1.6rem;
            margin-bottom: 10px;
        }

        .ad-content p {
            color: #555;
            margin-bottom: 20px;
            font-size: 0.95rem;
            line-height: 1.6;
        }

        /* Sections */
        .container {
            max-width: 1100px;
            margin: 40px auto;
            padding: 0 20px;
        }

        .section-title {
            text-align: center;
            margin-bottom: 30px;
        }

        .section-title h2 {
            font-size: 2rem;
            color: var(--primary-purple);
            position: relative;
            display: inline-block;
            padding-bottom: 10px;
        }

        .section-title h2::after {
            content: '';
            position: absolute;
            width: 60%;
            height: 4px;
            background-color: var(--accent-red);
            bottom: 0;
            left: 20%;
            border-radius: 2px;
        }

        /* Layanan Grid */
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 25px;
        }

        .service-box {
            background: white;
            border-radius: 10px;
            padding: 30px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.08);
            border-top: 5px solid var(--light-purple);
            transition: 0.3s;
        }

        .service-box:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 25px rgba(0,0,0,0.15);
            border-top-color: var(--accent-yellow);
        }

        .service-box i {
            font-size: 2.5rem;
            color: var(--accent-red);
            margin-bottom: 15px;
        }

        .service-box h3 {
            color: var(--primary-purple);
            margin-bottom: 10px;
            font-size: 1.25rem;
        }

        .service-box p {
            color: #666;
            font-size: 0.9rem;
            line-height: 1.5;
        }

        /* Galeri Proyek */
        .gallery-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 20px;
        }

        .gallery-item {
            background: white;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 4px 12px rgba(0,0,0,0.1);
            border: 2px solid #eee;
        }

        .gallery-item img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }

        .gallery-info {
            padding: 15px;
        }

        .gallery-info h4 {
            color: var(--primary-purple);
            font-size: 1.05rem;
            margin-bottom: 5px;
        }

        .gallery-info p {
            font-size: 0.85rem;
            color: #666;
        }

        /* YouTube Section */
        .youtube-section {
            background: linear-gradient(135deg, #2b0c2c, #4a154b);
            color: white;
            padding: 40px 20px;
            border-radius: 12px;
            text-align: center;
            margin: 40px 0;
            border: 3px solid var(--accent-yellow);
        }

        .youtube-section h3 {
            color: var(--accent-yellow);
            font-size: 1.8rem;
            margin-bottom: 10px;
        }

        .youtube-btn {
            display: inline-block;
            background: #ff0000;
            color: white;
            padding: 12px 25px;
            border-radius: 30px;
            text-decoration: none;
            font-weight: 700;
            margin-top: 15px;
            transition: 0.3s;
            box-shadow: 0 4px 10px rgba(0,0,0,0.3);
        }

        .youtube-btn:hover {
            background: #cc0000;
            transform: scale(1.05);
        }

        /* Kontak Admin */
        .contact-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 25px;
        }

        .contact-card {
            background: white;
            border-radius: 10px;
            padding: 30px;
            text-align: center;
            box-shadow: 0 5px 15px rgba(0,0,0,0.08);
            border-bottom: 5px solid var(--accent-yellow);
        }

        .contact-card h3 {
            color: var(--primary-purple);
            margin-bottom: 5px;
        }

        .contact-card .role {
            color: var(--accent-red);
            font-weight: 600;
            font-size: 0.9rem;
            margin-bottom: 15px;
            display: block;
        }

        .whatsapp-btn {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            gap: 8px;
            background: #25d366;
            color: white;
            padding: 12px 20px;
            border-radius: 5px;
            text-decoration: none;
            font-weight: 700;
            width: 100%;
            margin-top: 15px;
            transition: 0.3s;
        }

        .whatsapp-btn:hover {
            background: #1ebe5d;
        }

        /* Footer */
        footer {
            background: var(--primary-purple);
            color: white;
            text-align: center;
            padding: 20px;
            margin-top: 50px;
            border-top: 4px solid var(--accent-yellow);
            font-size: 0.9rem;
        }
    </style>
</head>
<body>

    <!-- Header & Navbar -->
    <header>
        <div class="navbar">
            <div class="logo">
                <i class="fa-solid fa-shield-halved" style="color: var(--accent-yellow);"></i>
                CAHAYA MITRA JAYA MANDIRI
            </div>
            <ul class="nav-links">
                <li><a href="#layanan">Layanan</a></li>
                <li><a href="#proyek">Hasil Proyek</a></li>
                <li><a href="#youtube">Channel YouTube</a></li>
                <li><a href="#kontak">Kontak Admin</a></li>
            </ul>
        </div>
    </header>

    <!-- Hero Banner Utama -->
    <section class="hero-banner">
        <h1>CAHAYA MITRA JAYA MANDIRI</h1>
        <p>Pusat Distributor, Supplier & Kontraktor Terpercaya untuk Pagar BRC, Kawat Silet, Kawat Duri, serta Jasa Bangun dan Renovasi Rumah.</p>
    </section>

    <!-- Iklan Gudang & Foto Produk -->
    <div class="ad-section">
        <div class="ad-card">
            <div class="ad-image">
                <!-- Foto Anda dengan tumpukan stok pagar BRC -->
                <img src="1000227170.jpg" alt="Stok Pagar BRC Gudang Cahaya Mitra Jaya Mandiri">
            </div>
            <div class="ad-content">
                <span class="badge-promo"><i class="fa-solid fa-fire"></i> Ready Stock Distributor</span>
                <h2>Pusat Penjualan & Jasa Pasang Pagar BRC Berkualitas</h2>
                <p>Kami menyediakan suplai material dan jasa pemasangan langsung dari gudang: **Pagar BRC hot-dip & electroplating**, **Kawat Silet (Razor Wire)**, serta **Kawat Duri** berkualitas tinggi untuk keamanan pabrik, perumahan, dan lahan Anda.</p>
                <a href="https://wa.me/6283829449983?text=Halo%20Ibu%20Vina,%20saya%20tertarik%20dengan%20penawaran%20pagar%20BRC%20dan%20jasa%20konstruksi." class="whatsapp-btn" target="_blank">
                    <i class="fa-brands fa-whatsapp"></i> Konsultasi & Pesan Sekarang
                </a>
            </div>
        </div>
    </div>

    <!-- Layanan Kami -->
    <div class="container" id="layanan">
        <div class="section-title">
            <h2>Layanan Utama Kami</h2>
        </div>
        <div class="services-grid">
            <div class="service-box">
                <i class="fa-solid fa-helmet-safety"></i>
                <h3>Bangun Rumah Dari Nol</h3>
                <p>Melayani pembangunan rumah hunian, ruko, atau gedung dari tahap perencanaan, persiapan lahan, hingga finishing siap huni dengan tenaga ahli berpengalaman.</p>
            </div>
            <div class="service-box">
                <i class="fa-solid fa-house-chimney-crack"></i>
                <h3>Renovasi Rumah & Gedung</h3>
                <p>Solusi tuntas renovasi skala kecil maupun besar: perbaikan atap, penambahan ruangan, pengecatan, bongkar pasang struktur, hingga peremajaan tampilan bangunan.</p>
            </div>
            <div class="service-box">
                <i class="fa-solid fa-bars-staggered"></i>
                <h3>Pagar BRC, Kawat Silet & Duri</h3>
                <p>Spesialis penyediaan material dan jasa pasang profesional untuk pagar BRC berbagai ukuran, kawat silet anti-maling, serta kawat duri pengaman perimeter.</p>
            </div>
        </div>
    </div>

    <!-- Contoh Hasil Pengerjaan Proyek -->
    <div class="container" id="proyek">
        <div class="section-title">
            <h2>Contoh Hasil Pengerjaan Proyek</h2>
        </div>
        <div class="gallery-grid">
            <div class="gallery-item">
                <img src="https://images.unsplash.com/photo-1513694203232-719a280e022f?auto=format&fit=crop&w=600&q=80" alt="Bangun Rumah">
                <div class="gallery-info">
                    <h4>Proyek Bangun Rumah Minimalis</h4>
                    <p>Pembangunan struktur dari nol hingga serah terima kunci di wilayah Jabodetabek.</p>
                </div>
            </div>
            <div class="gallery-item">
                <img src="https://images.unsplash.com/photo-1503387762-592deb58ef4e?auto=format&fit=crop&w=600&q=80" alt="Renovasi">
                <div class="gallery-info">
                    <h4>Renovasi & Perluasan Ruangan</h4>
                    <p>Peremajaan tata letak dan renovasi total tampak depan bangunan komersial.</p>
                </div>
            </div>
            <div class="gallery-item">
                <img src="https://images.unsplash.com/photo-1558445101-729c7809968a?auto=format&fit=crop&w=600&q=80" alt="Pagar BRC">
                <div class="gallery-info">
                    <h4>Pemasangan Pagar BRC & Kawat Silet</h4>
                    <p>Instalasi pengamanan keliling lahan gudang dan perumahan menggunakan pagar BRC & kawat silet.</p>
                </div>
            </div>
        </div>
    </div>

    <!-- YouTube Section -->
    <div class="container" id="youtube">
        <div class="youtube-section">
            <i class="fa-brands fa-youtube" style="font-size: 3.5rem; color: #ff0000; margin-bottom: 10px;"></i>
            <h3>Dokumentasi Lapangan & Tutorial</h3>
            <p>Saksikan proses kerja nyata, tips konstruksi, dan aksi pemasangan di channel YouTube resmi kami:</p>
            <h2 style="color: #fff; margin: 10px 0;">CAHAYA BOSS KULI</h2>
            <a href="https://www.youtube.com/@cahayabosskuli" class="youtube-btn" target="_blank">
                <i class="fa-brands fa-youtube"></i> Kunjungi Channel YouTube
            </a>
        </div>
    </div>

    <!-- Kontak Admin / Pemesanan -->
    <div class="container" id="kontak">
        <div class="section-title">
            <h2>Hubungi Admin Kami</h2>
        </div>
        <div class="contact-container">
            <!-- Admin Cewek -->
            <div class="contact-card">
                <i class="fa-solid fa-headset" style="font-size: 2.5rem; color: var(--light-purple); margin-bottom: 10px;"></i>
                <h3>IBU VINA</h3>
                <span class="role">Admin & Layanan Pelanggan</span>
                <p><i class="fa-solid fa-phone"></i> +62 838-2944-9983</p>
                <a href="https://wa.me/6283829449983?text=Halo%20Ibu%20Vina,%20saya%20ingin%20berkonsultasi%20mengenai%20jasa%20dan%20produk%20Cahaya%20Mitra%20Jaya%20Mandiri." class="whatsapp-btn" target="_blank">
                    <i class="fa-brands fa-whatsapp"></i> Chat WhatsApp Vina
                </a>
            </div>

            <!-- Admin Cowok -->
            <div class="contact-card">
                <i class="fa-solid fa-user-gear" style="font-size: 2.5rem; color: var(--accent-red); margin-bottom: 10px;"></i>
                <h3>PAK FERDY</h3>
                <span class="role">Marketing & Pengukuran Lapangan</span>
                <p><i class="fa-solid fa-phone"></i> 0882-1432-1193</p>
                <a href="https://wa.me/6288214321193?text=Halo%20Pak%20Ferdy,%20saya%20ingin%20memesan%20pagar%20BRC%20dan%20survei%20lokasi." class="whatsapp-btn" target="_blank">
                    <i class="fa-brands fa-whatsapp"></i> Chat WhatsApp Ferdy
                </a>
            </div>
        </div>
    </div>

    <!-- Footer -->
    <footer>
        <p>&copy; 2026 CAHAYA MITRA JAYA MANDIRI. All Rights Reserved.</p>
        <p style="font-size: 0.8rem; color: #ffb300; margin-top: 5px;">Pusat Distributor Pagar BRC & Kontraktor Bangunan Terpercaya</p>
    </footer>

</body>
</html>
