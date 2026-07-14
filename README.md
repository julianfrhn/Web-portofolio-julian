# Web-portofolio-julian
<!DOCTYPE html>
<html lang="id" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Julian Farhan Wijaya - Portfolio</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Font Awesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
    
    <script>
        tailwind.config = {
            darkMode: 'class',
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Plus Jakarta Sans', 'sans-serif'],
                    },
                    colors: {
                        brand: {
                            50: '#f0f7ff',
                            100: '#e0effe',
                            500: '#0284c7',
                            600: '#0369a1',
                            700: '#075985',
                            900: '#0c4a6e',
                        }
                    }
                }
            }
        }
    </script>
    <style>
        /* Efek transisi global untuk pergantian tema */
        * {
            transition: background-color 0.3s ease, border-color 0.3s ease, text-decoration 0.3s ease;
        }
    </style>
</head>
<body class="bg-slate-50 text-slate-800 dark:bg-slate-900 dark:text-slate-100 min-h-screen font-sans">

    <!-- HEADER / NAVIGATION -->
    <nav class="fixed top-0 left-0 right-0 z-50 bg-white/80 dark:bg-slate-900/80 backdrop-blur-md border-b border-slate-200 dark:border-slate-800">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex items-center justify-between h-16">
                <!-- Logo -->
                <div class="flex-shrink-0 flex items-center">
                    <span class="text-xl font-extrabold tracking-wider bg-gradient-to-r from-brand-600 to-sky-400 bg-clip-text text-transparent">
                        JFW.
                    </span>
                </div>
                
                <!-- Desktop Navigasi -->
                <div class="hidden md:flex items-center space-x-8">
                    <a href="#beranda" class="text-sm font-medium hover:text-brand-500 transition-colors">Beranda</a>
                    <a href="#tentang" class="text-sm font-medium hover:text-brand-500 transition-colors">Tentang Saya</a>
                    <a href="#pengalaman" class="text-sm font-medium hover:text-brand-500 transition-colors">Pengalaman</a>
                    <a href="#keahlian" class="text-sm font-medium hover:text-brand-500 transition-colors">Keahlian</a>
                    <a href="#proyek" class="text-sm font-medium hover:text-brand-500 transition-colors">Alat & Proyek</a>
                    <a href="#kontak" class="text-sm font-medium hover:text-brand-500 transition-colors">Kontak</a>
                </div>

                <!-- Kontrol & Tema Toggle -->
                <div class="flex items-center space-x-4">
                    <!-- Dark Mode Button -->
                    <button id="themeToggle" class="p-2 rounded-full hover:bg-slate-100 dark:hover:bg-slate-800 text-slate-600 dark:text-slate-300 transition-colors" aria-label="Toggle Theme">
                        <i id="themeIcon" class="fa-solid fa-moon text-lg"></i>
                    </button>
                    
                    <!-- Hubungi Button -->
                    <a href="#kontak" class="hidden sm:inline-flex items-center px-4 py-2 border border-transparent text-sm font-semibold rounded-lg text-white bg-brand-600 hover:bg-brand-700 transition shadow-sm">
                        Hubungi Saya
                    </a>

                    <!-- Mobile Menu Button -->
                    <button id="mobileMenuBtn" class="md:hidden p-2 rounded-lg hover:bg-slate-100 dark:hover:bg-slate-800 text-slate-600 dark:text-slate-300" aria-label="Buka Menu">
                        <i class="fa-solid fa-bars text-xl"></i>
                    </button>
                </div>
            </div>
        </div>

        <!-- Mobile Navigasi -->
        <div id="mobileMenu" class="hidden md:hidden border-b border-slate-200 dark:border-slate-800 bg-white dark:bg-slate-900 px-4 pt-2 pb-4 space-y-1">
            <a href="#beranda" class="block px-3 py-2 rounded-md text-base font-medium hover:bg-slate-100 dark:hover:bg-slate-800">Beranda</a>
            <a href="#tentang" class="block px-3 py-2 rounded-md text-base font-medium hover:bg-slate-100 dark:hover:bg-slate-800">Tentang Saya</a>
            <a href="#pengalaman" class="block px-3 py-2 rounded-md text-base font-medium hover:bg-slate-100 dark:hover:bg-slate-800">Pengalaman</a>
            <a href="#keahlian" class="block px-3 py-2 rounded-md text-base font-medium hover:bg-slate-100 dark:hover:bg-slate-800">Keahlian</a>
            <a href="#proyek" class="block px-3 py-2 rounded-md text-base font-medium hover:bg-slate-100 dark:hover:bg-slate-800">Alat & Proyek</a>
            <a href="#kontak" class="block px-3 py-2 rounded-md text-base font-medium hover:bg-slate-100 dark:hover:bg-slate-800">Kontak</a>
            <a href="#kontak" class="block text-center w-full mt-2 px-4 py-2 text-sm font-semibold rounded-lg text-white bg-brand-600">Hubungi Saya</a>
        </div>
    </nav>

    <!-- HERO SECTION -->
    <section id="beranda" class="pt-32 pb-20 overflow-hidden relative">
        <div class="absolute inset-0 bg-gradient-to-tr from-brand-50/30 to-sky-100/10 dark:from-brand-950/20 dark:to-slate-900 -z-10"></div>
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="lg:grid lg:grid-cols-12 lg:gap-8 items-center">
                <!-- Teks Hero -->
                <div class="sm:text-center md:max-w-2xl md:mx-auto lg:col-span-7 lg:text-left">
                    <span class="inline-flex items-center px-3 py-1 rounded-full text-sm font-medium bg-brand-100 text-brand-600 dark:bg-brand-900/40 dark:text-brand-300 mb-4 animate-pulse">
                        <i class="fa-solid fa-briefcase mr-1.5"></i> Procurement
                    </span>
                    <h1 class="text-4xl sm:text-5xl lg:text-6xl font-extrabold tracking-tight">
                        <span class="block">Halo, Saya</span>
                        <span class="block text-brand-600 dark:text-brand-500 mt-1">Julian Farhan Wijaya</span>
                    </h1>
                    <p class="mt-4 text-lg text-slate-600 dark:text-slate-300 leading-relaxed">
                        Menghubungkan logika pemikiran analitis dari latar belakang <strong class="text-slate-800 dark:text-white">S1 Informatika</strong> dengan keahlian praktis <strong class="text-slate-800 dark:text-white">Procurement</strong>. Berpengalaman dalam melakukan negosiasi strategis, analisis data rantai pasok, dan manajemen vendor guna mendorong efisiensi anggaran maksimal.
                    </p>
                    
                    <div class="mt-8 sm:max-w-lg sm:mx-auto lg:mx-0 flex flex-col sm:flex-row gap-4 justify-center lg:justify-start">
                        <a href="#kontak" class="inline-flex items-center justify-center px-6 py-3 border border-transparent text-base font-bold rounded-xl text-white bg-brand-600 hover:bg-brand-700 transition shadow-lg shadow-brand-500/20">
                            <i class="fa-solid fa-paper-plane mr-2"></i> Rekrut Saya
                        </a>
                        <button onclick="downloadResumeSimulator()" class="inline-flex items-center justify-center px-6 py-3 border border-slate-300 dark:border-slate-700 text-base font-bold rounded-xl bg-white dark:bg-slate-800 hover:bg-slate-50 dark:hover:bg-slate-700 transition">
                            <i class="fa-solid fa-file-arrow-down mr-2"></i> Unduh CV (PDF)
                        </button>
                    </div>

                    <!-- Kontak Ringkas -->
                    <div class="mt-10 pt-8 border-t border-slate-200 dark:border-slate-800 grid grid-cols-2 sm:grid-cols-3 gap-4 text-sm text-slate-500 dark:text-slate-400">
                        <div class="flex items-center gap-2">
                            <i class="fa-solid fa-location-dot text-brand-500"></i>
                            <span>Tangerang Selatan, ID</span>
                        </div>
                        <div class="flex items-center gap-2">
                            <i class="fa-solid fa-envelope text-brand-500"></i>
                            <span>julianfarhan12345@gmail.com</span>
                        </div>
                        <div class="flex items-center gap-2 col-span-2 sm:col-span-1">
                            <i class="fa-brands fa-linkedin text-brand-500"></i>
                            <a href="https://linkedin.com/in/julianfarhan/" target="_blank" class="hover:underline">/in/julianfarhan</a>
                        </div>
                    </div>
                </div>

                <!-- Ilustrasi Visual -->
                <div class="mt-12 sm:mt-16 lg:mt-0 lg:col-span-5 flex justify-center">
                    <div class="relative w-72 h-72 sm:w-96 sm:h-96">
                        <!-- Ornamen Lingkaran Belakang -->
                        <div class="absolute inset-0 rounded-full bg-gradient-to-tr from-brand-500 to-sky-300 opacity-20 blur-2xl animate-spin-slow"></div>
                        <!-- Frame Gambar Utama -->
                        <div class="absolute inset-4 rounded-3xl bg-slate-800/5 dark:bg-slate-700/20 border border-slate-200 dark:border-slate-800 shadow-2xl overflow-hidden flex flex-col justify-between p-6">
                            <div class="flex justify-between items-center">
                                <div class="flex space-x-1.5">
                                    <span class="w-3 h-3 rounded-full bg-red-500"></span>
                                    <span class="w-3 h-3 rounded-full bg-yellow-500"></span>
                                    <span class="w-3 h-3 rounded-full bg-green-500"></span>
                                </div>
                                <span class="text-xs text-slate-400 dark:text-slate-500 font-mono">portfolio.py</span>
                            </div>
                            
                            <div class="my-auto font-mono text-xs sm:text-sm text-brand-600 dark:text-sky-400 space-y-2">
                                <p><span class="text-slate-400"># Profil Singkat</span></p>
                                <p><span class="text-pink-500">class</span> <span class="text-amber-500">JulianFarhan</span>:</p>
                                <p class="pl-4">def __init__(self):</p>
                                <p class="pl-8">self.role = <span class="text-green-500">"Procurement & IT Analyst"</span></p>
                                <p class="pl-8">self.edu = <span class="text-green-500">"Telkom University"</span></p>
                                <p class="pl-8">self.gpa = <span class="text-green-500">2.91</span></p>
                                <p class="pl-8">self.skills = [<span class="text-green-500">"Negotiation"</span>, <span class="text-green-500">"Data Analyst"</span>]</p>
                                <p class="pl-4">def handle_cost_saving(self):</p>
                                <p class="pl-8">return self.skills.maximize_efficiency()</p>
                            </div>

                            <div class="border-t border-slate-200 dark:border-slate-800 pt-4 flex justify-between items-center">
                                <div class="flex items-center gap-2">
                                    <div class="w-2.5 h-2.5 rounded-full bg-emerald-500 animate-pulse"></div>
                                    <span class="text-xs text-slate-500">Ready to Negotiate</span>
                                </div>
                                <i class="fa-solid fa-code text-slate-400"></i>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- TENTANG SAYA -->
    <section id="tentang" class="py-20 bg-white dark:bg-slate-900/50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <h2 class="text-3xl font-extrabold sm:text-4xl text-slate-900 dark:text-white">Tentang Saya</h2>
                <div class="w-16 h-1 bg-brand-500 mx-auto mt-4 rounded-full"></div>
                <p class="mt-4 text-slate-600 dark:text-slate-400 text-lg">
                    Seorang profesional yang berambisi menjadi jembatan antara efisiensi bisnis dan teknologi masa kini.
                </p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 gap-12 items-center">
                <div class="space-y-6">
                    <h3 class="text-2xl font-bold text-slate-900 dark:text-white">Menghubungkan Ilmu IT dengan Dunia Pengadaan</h3>
                    <p class="text-slate-600 dark:text-slate-300 leading-relaxed">
                        Lulus dari <strong class="text-slate-800 dark:text-white">Telkom University</strong> jurusan S1 Informatika memberi saya landasan berpikir yang sangat kuat dalam struktur logika, analisis big data, dan penyelesaian masalah secara sistematis. 
                    </p>
                    <p class="text-slate-600 dark:text-slate-300 leading-relaxed">
                        Dengan pengalaman lebih dari 2 tahun di bidang pengadaan trading dan cold storage, saya berfokus untuk tidak sekadar "membeli", melainkan menggunakan pendekatan analitik guna menakar risiko pemasok, menyusun strategi efisiensi biaya, serta mengotomatisasi SOP guna mengeliminasi miskomunikasi.
                    </p>
                    <div class="grid grid-cols-2 gap-4 pt-4">
                        <div class="p-4 bg-slate-50 dark:bg-slate-800 rounded-xl">
                            <span class="block text-3xl font-extrabold text-brand-600 dark:text-brand-500">2+</span>
                            <span class="text-sm text-slate-500">Tahun Pengalaman</span>
                        </div>
                        <div class="p-4 bg-slate-50 dark:bg-slate-800 rounded-xl">
                            <span class="block text-3xl font-extrabold text-brand-600 dark:text-brand-500">Informatika</span>
                            <span class="text-sm text-slate-500">Dasar Pemecahan Masalah</span>
                        </div>
                    </div>
                </div>

                <!-- Bagian Kanan: Fokus Nilai -->
                <div class="bg-gradient-to-br from-slate-50 to-slate-100 dark:from-slate-800/50 dark:to-slate-800 p-8 rounded-2xl border border-slate-200 dark:border-slate-700 space-y-6">
                    <h4 class="text-lg font-bold text-slate-900 dark:text-white uppercase tracking-wider text-brand-600 dark:text-brand-400">Prinsip Kerja Saya</h4>
                    
                    <div class="flex items-start gap-4">
                        <div class="w-10 h-10 rounded-lg bg-brand-100 dark:bg-brand-900/50 text-brand-600 dark:text-brand-300 flex items-center justify-center shrink-0">
                            <i class="fa-solid fa-comments-dollar"></i>
                        </div>
                        <div>
                            <h5 class="font-bold text-slate-900 dark:text-white">Negosiasi Bernilai Tinggi</h5>
                            <p class="text-sm text-slate-500 dark:text-slate-400 mt-1">Mengejar hasil win-win yang menjamin kualitas terbaik serta tenggat pembayaran yang fleksibel bagi perusahaan.</p>
                        </div>
                    </div>

                    <div class="flex items-start gap-4">
                        <div class="w-10 h-10 rounded-lg bg-brand-100 dark:bg-brand-900/50 text-brand-600 dark:text-brand-300 flex items-center justify-center shrink-0">
                            <i class="fa-solid fa-route"></i>
                        </div>
                        <div>
                            <h5 class="font-bold text-slate-900 dark:text-white">Manajemen Pemasok Strategis</h5>
                            <p class="text-sm text-slate-500 dark:text-slate-400 mt-1">Mengidentifikasi kemitraan jangka panjang demi keberlangsungan rantai pasok bebas kendala.</p>
                        </div>
                    </div>

                    <div class="flex items-start gap-4">
                        <div class="w-10 h-10 rounded-lg bg-brand-100 dark:bg-brand-900/50 text-brand-600 dark:text-brand-300 flex items-center justify-center shrink-0">
                            <i class="fa-solid fa-clipboard-check"></i>
                        </div>
                        <div>
                            <h5 class="font-bold text-slate-900 dark:text-white">Penyusunan SOP & Efisiensi</h5>
                            <p class="text-sm text-slate-500 dark:text-slate-400 mt-1">Mengembangkan SOP pengadaan berbasis kolaboratif untuk mempercepat waktu respons internal.</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- PENGALAMAN KERJA & PENDIDIKAN -->
    <section id="pengalaman" class="py-20 bg-slate-50 dark:bg-slate-900">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <h2 class="text-3xl font-extrabold sm:text-4xl text-slate-900 dark:text-white">Riwayat Karir & Studi</h2>
                <div class="w-16 h-1 bg-brand-500 mx-auto mt-4 rounded-full"></div>
                <p class="mt-4 text-slate-600 dark:text-slate-400 text-lg">
                    Langkah perjalanan profesional saya dalam industri procurement dan teknologi.
                </p>
            </div>

            <div class="grid grid-cols-1 lg:grid-cols-12 gap-12">
                <!-- Pengalaman Kerja (Kiri - 7 Kolom) -->
                <div class="lg:col-span-7 space-y-8">
                    <h3 class="text-xl font-bold flex items-center gap-2 mb-6">
                        <i class="fa-solid fa-briefcase text-brand-500"></i> Pengalaman Kerja
                    </h3>
                    
                    <div class="relative pl-6 border-l-2 border-slate-200 dark:border-slate-800 space-y-12">
                        <!-- PT Rukma Perdana Niaga -->
                        <div class="relative">
                            <!-- Titik Penunjuk -->
                            <div class="absolute -left-[31px] top-1.5 w-4 h-4 rounded-full bg-brand-500 border-4 border-white dark:border-slate-900"></div>
                            <div class="flex flex-col sm:flex-row justify-between items-start sm:items-center mb-2">
                                <h4 class="font-bold text-lg text-slate-900 dark:text-white">Procurement Trading & Coldstorage</h4>
                                <span class="text-xs font-semibold px-2.5 py-1 rounded bg-brand-100 text-brand-700 dark:bg-brand-900/40 dark:text-brand-300 mt-1 sm:mt-0">April 2024 - Oktober 2025</span>
                            </div>
                            <p class="text-sm font-semibold text-slate-500 dark:text-slate-400 mb-3">PT Rukma Perdana Niaga (RPT Group) | Surabaya</p>
                            <ul class="space-y-2 text-sm text-slate-600 dark:text-slate-300 list-disc list-inside">
                                <li>Melakukan negosiasi dengan pemasok untuk mendapatkan harga, kualitas, dan persyaratan pembayaran yang paling menguntungkan bagi Perusahaan.</li>
                                <li>Mengidentifikasi dan mencari pemasok strategis yang dapat mendukung kebutuhan jangka panjang dan efisiensi rantai pasokan.</li>
                                <li>Merencanakan dan mengelola anggaran pengadaan secara efektif agar selaras dengan target biaya dan kebutuhan operasional.</li>
                                <li>Membangun dan memelihara kemitraan kolaboratif dengan perusahaan terkait, termasuk mitra bisnis dan vendor, untuk kelancaran operasi bisnis.</li>
                                <li>Membangun SOP pengadaan untuk memastikan tidak terjadinya miskomunikasi antar tim.</li>
                            </ul>
                        </div>

                        <!-- Voice Lounge and Cafe -->
                        <div class="relative">
                            <!-- Titik Penunjuk -->
                            <div class="absolute -left-[31px] top-1.5 w-4 h-4 rounded-full bg-slate-300 dark:bg-slate-700 border-4 border-white dark:border-slate-900"></div>
                            <div class="flex flex-col sm:flex-row justify-between items-start sm:items-center mb-2">
                                <h4 class="font-bold text-lg text-slate-900 dark:text-white">Captain</h4>
                                <span class="text-xs font-semibold px-2.5 py-1 rounded bg-slate-100 text-slate-700 dark:bg-slate-800 dark:text-slate-300 mt-1 sm:mt-0">Maret 2023 - Agustus 2023</span>
                            </div>
                            <p class="text-sm font-semibold text-slate-500 dark:text-slate-400 mb-3">Voice Lounge and Cafe | Bandung</p>
                            <ul class="space-y-2 text-sm text-slate-600 dark:text-slate-300 list-disc list-inside">
                                <li>Memimpin dan memotivasi tim serta mengatur strategi pemasaran yang bertujuan untuk meningkatkan penjualan dan kinerja tim.</li>
                                <li>Mengarahkan tim untuk terus berkembang demi kepuasan pelanggan secara konstan.</li>
                                <li>Merencanakan dan menyusun acara yang akan datang demi menyokong sasaran pemasaran dan bisnis.</li>
                                <li>Memastikan ditaatinya SOP melalui pengawasan dan pembinaan terhadap operasional harian tim.</li>
                            </ul>
                        </div>

                        <!-- Bandung Techno Park -->
                        <div class="relative">
                            <!-- Titik Penunjuk -->
                            <div class="absolute -left-[31px] top-1.5 w-4 h-4 rounded-full bg-slate-300 dark:bg-slate-700 border-4 border-white dark:border-slate-900"></div>
                            <div class="flex flex-col sm:flex-row justify-between items-start sm:items-center mb-2">
                                <h4 class="font-bold text-lg text-slate-900 dark:text-white">System Analyst (Magang)</h4>
                                <span class="text-xs font-semibold px-2.5 py-1 rounded bg-slate-100 text-slate-700 dark:bg-slate-800 dark:text-slate-300 mt-1 sm:mt-0">Juli 2020 - Agustus 2020</span>
                            </div>
                            <p class="text-sm font-semibold text-slate-500 dark:text-slate-400 mb-3">Bandung Techno Park | Kab. Bandung</p>
                            <ul class="space-y-2 text-sm text-slate-600 dark:text-slate-300 list-disc list-inside">
                                <li>Mengumpulkan dan menganalisis dataset pengguna Xgracias Lite.</li>
                                <li>Membuat rancangan modul dan field sistem secara detail untuk mendukung pengembangan perangkat lunak.</li>
                            </ul>
                        </div>
                    </div>
                </div>

                <!-- Pendidikan & Akademik (Kanan - 5 Kolom) -->
                <div class="lg:col-span-5 space-y-8">
                    <div>
                        <h3 class="text-xl font-bold flex items-center gap-2 mb-6">
                            <i class="fa-solid fa-graduation-cap text-brand-500"></i> Pendidikan
                        </h3>
                        <div class="bg-white dark:bg-slate-800 p-6 rounded-2xl border border-slate-200 dark:border-slate-700 shadow-sm relative overflow-hidden">
                            <div class="absolute right-0 top-0 w-24 h-24 bg-brand-500/5 rounded-bl-full pointer-events-none"></div>
                            <span class="text-xs font-bold text-brand-600 dark:text-brand-400 uppercase tracking-wider block mb-1">Sarjana Komputer</span>
                            <h4 class="font-bold text-lg text-slate-900 dark:text-white">Universitas Telkom</h4>
                            <p class="text-sm text-slate-500 dark:text-slate-400 mt-1">S1 Informatika | IPK 2.91</p>
                            <p class="text-xs text-slate-400 mt-1">Tahun Kelulusan: 2017 - 2023</p>
                            
                            <div class="mt-4 pt-4 border-t border-slate-100 dark:border-slate-700">
                                <span class="text-xs font-bold text-slate-700 dark:text-slate-300 block mb-1">Tugas Akhir:</span>
                                <p class="text-xs italic text-slate-600 dark:text-slate-400 leading-relaxed">
                                    "Sentimen Analisis Review Restoran Bakmie di Bandung Menggunakan Metode Machine Learning" (Publikasi Jurnal & Terdaftar Hak Kekayaan Intelektual - HKI)
                                </p>
                            </div>
                            <div class="mt-3 text-xs bg-slate-50 dark:bg-slate-900 p-2 rounded text-slate-500 flex items-center gap-2">
                                <i class="fa-solid fa-users text-brand-500"></i>
                                <span>Anggota Eksternal Organisasi (GIGABYTE)</span>
                            </div>
                        </div>
                    </div>

                    <!-- Highlight Spesial: Kenapa Kombinasi JFW Berharga? -->
                    <div class="bg-gradient-to-r from-brand-600 to-sky-600 p-6 rounded-2xl text-white shadow-lg shadow-brand-600/10">
                        <h4 class="font-bold text-lg flex items-center gap-2">
                            <i class="fa-solid fa-lightbulb"></i> Perspektif Unik
                        </h4>
                        <p class="text-sm text-brand-100 mt-2 leading-relaxed">
                            Sebagai Sarjana Informatika yang berkarir di Procurement, saya memiliki keunggulan kompetitif berupa kemampuan mengotomatisasi visualisasi data anggaran, menggunakan logika pemrograman untuk menyusun kueri audit vendor, dan menganalisis kepuasan layanan dengan pemodelan sentimen data.
                        </p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- KEAHLIAN -->
    <section id="keahlian" class="py-20 bg-white dark:bg-slate-900/50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <h2 class="text-3xl font-extrabold sm:text-4xl text-slate-900 dark:text-white">Peta Keahlian</h2>
                <div class="w-16 h-1 bg-brand-500 mx-auto mt-4 rounded-full"></div>
                <p class="mt-4 text-slate-600 dark:text-slate-400 text-lg">
                    Daftar keahlian multi-disiplin yang saya kuasai dan aplikasikan dalam pekerjaan.
                </p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <!-- Procurement & Business -->
                <div class="bg-slate-50 dark:bg-slate-800/80 p-6 rounded-2xl border border-slate-200 dark:border-slate-700/60 shadow-sm">
                    <div class="w-12 h-12 rounded-xl bg-amber-100 dark:bg-amber-900/40 text-amber-600 dark:text-amber-300 flex items-center justify-center mb-6">
                        <i class="fa-solid fa-chart-line text-xl"></i>
                    </div>
                    <h3 class="text-lg font-bold text-slate-900 dark:text-white mb-4">Pengadaan & Bisnis</h3>
                    <ul class="space-y-3">
                        <li class="flex items-center justify-between text-sm">
                            <span class="text-slate-600 dark:text-slate-300">Direct Procurement</span>
                            <span class="font-semibold text-brand-600">Expert</span>
                        </li>
                        <li class="flex items-center justify-between text-sm">
                            <span class="text-slate-600 dark:text-slate-300">Indirect Procurement</span>
                            <span class="font-semibold text-brand-600">Advanced</span>
                        </li>
                        <li class="flex items-center justify-between text-sm">
                            <span class="text-slate-600 dark:text-slate-300">Hubungan Vendor</span>
                            <span class="font-semibold text-brand-600">Advanced</span>
                        </li>
                        <li class="flex items-center justify-between text-sm">
                            <span class="text-slate-600 dark:text-slate-300">Manajemen Anggaran</span>
                            <span class="font-semibold text-brand-600">Advanced</span>
                        </li>
                        <li class="flex items-center justify-between text-sm">
                            <span class="text-slate-600 dark:text-slate-300">Pemasaran & Manajemen</span>
                            <span class="font-semibold text-brand-600">Intermediate</span>
                        </li>
                    </ul>
                </div>

                <!-- Tech & Software Skills -->
                <div class="bg-slate-50 dark:bg-slate-800/80 p-6 rounded-2xl border border-slate-200 dark:border-slate-700/60 shadow-sm">
                    <div class="w-12 h-12 rounded-xl bg-brand-100 dark:bg-brand-900/40 text-brand-600 dark:text-brand-300 flex items-center justify-center mb-6">
                        <i class="fa-solid fa-laptop-code text-xl"></i>
                    </div>
                    <h3 class="text-lg font-bold text-slate-900 dark:text-white mb-4">Sistem & Perangkat Lunak</h3>
                    <ul class="space-y-3">
                        <li class="flex items-center justify-between text-sm">
                            <span class="text-slate-600 dark:text-slate-300">Microsoft Office (Excel/Word)</span>
                            <span class="font-semibold text-brand-600">Expert</span>
                        </li>
                        <li class="flex items-center justify-between text-sm">
                            <span class="text-slate-600 dark:text-slate-300">Python (Machine Learning)</span>
                            <span class="font-semibold text-brand-600">Advanced</span>
                        </li>
                        <li class="flex items-center justify-between text-sm">
                            <span class="text-slate-600 dark:text-slate-300">Sistem Basis Data (SQL)</span>
                            <span class="font-semibold text-brand-600">Advanced</span>
                        </li>
                        <li class="flex items-center justify-between text-sm">
                            <span class="text-slate-600 dark:text-slate-300">Web Dev (JS, HTML, PHP, CSS)</span>
                            <span class="font-semibold text-brand-600">Intermediate</span>
                        </li>
                        <li class="flex items-center justify-between text-sm">
                            <span class="text-slate-600 dark:text-slate-300">Desain (Canva, Adobe)</span>
                            <span class="font-semibold text-brand-600">Advanced</span>
                        </li>
                    </ul>
                </div>

                <!-- Interpersonal -->
                <div class="bg-slate-50 dark:bg-slate-800/80 p-6 rounded-2xl border border-slate-200 dark:border-slate-700/60 shadow-sm">
                    <div class="w-12 h-12 rounded-xl bg-emerald-100 dark:bg-emerald-900/40 text-emerald-600 dark:text-emerald-300 flex items-center justify-center mb-6">
                        <i class="fa-solid fa-users text-xl"></i>
                    </div>
                    <h3 class="text-lg font-bold text-slate-900 dark:text-white mb-4">Kemampuan Interpersonal</h3>
                    <ul class="space-y-3">
                        <li class="flex items-center justify-between text-sm">
                            <span class="text-slate-600 dark:text-slate-300">Kemampuan Negosiasi</span>
                            <span class="font-semibold text-brand-600">Expert</span>
                        </li>
                        <li class="flex items-center justify-between text-sm">
                            <span class="text-slate-600 dark:text-slate-300">Kepemimpinan Tim</span>
                            <span class="font-semibold text-brand-600">Expert</span>
                        </li>
                        <li class="flex items-center justify-between text-sm">
                            <span class="text-slate-600 dark:text-slate-300">Komunikasi Efektif</span>
                            <span class="font-semibold text-brand-600">Expert</span>
                        </li>
                        <li class="flex items-center justify-between text-sm">
                            <span class="text-slate-600 dark:text-slate-300">Pemecahan Masalah</span>
                            <span class="font-semibold text-brand-600">Advanced</span>
                        </li>
                        <li class="flex items-center justify-between text-sm">
                            <span class="text-slate-600 dark:text-slate-300">Kerja Tim & Manajemen Waktu</span>
                            <span class="font-semibold text-brand-600">Advanced</span>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- ALAT & PROYEK INTERAKTIF -->
    <section id="proyek" class="py-20 bg-slate-100 dark:bg-slate-900">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <h2 class="text-3xl font-extrabold sm:text-4xl text-slate-900 dark:text-white">Alat & Proyek Interaktif</h2>
                <div class="w-16 h-1 bg-brand-500 mx-auto mt-4 rounded-full"></div>
                <p class="mt-4 text-slate-600 dark:text-slate-400 text-lg">
                    Berikut adalah bentuk interaksi nyata dari penerapan ilmu IT dan Procurement saya yang bisa Anda uji coba langsung di halaman ini.
                </p>
            </div>

            <div class="grid grid-cols-1 lg:grid-cols-2 gap-12">
                <!-- ALAT 1: SIMULATOR ANALISIS SENTIMEN REVIEW RESTORAN -->
                <div class="bg-white dark:bg-slate-800 p-8 rounded-3xl border border-slate-200 dark:border-slate-700 shadow-lg relative overflow-hidden">
                    <span class="absolute top-4 right-4 text-xs font-mono px-2 py-1 rounded bg-indigo-50 dark:bg-indigo-950/50 text-indigo-600 dark:text-indigo-400">
                        Topik Tugas Akhir (Informatika)
                    </span>
                    <h3 class="text-xl font-bold text-slate-900 dark:text-white flex items-center gap-2">
                        <i class="fa-solid fa-face-smile text-indigo-500"></i> Simulator Analisis Sentimen Restoran
                    </h3>
                    <p class="text-sm text-slate-500 dark:text-slate-400 mt-2">
                        Tugas akhir saya berfokus pada analisis opini pelanggan di Bandung menggunakan Machine Learning. Masukkan ulasan Anda di bawah ini untuk melihat bagaimana algoritma menyimpulkan maknanya.
                    </p>

                    <!-- Area Input Review -->
                    <div class="mt-6 space-y-4">
                        <div>
                            <label for="sentimentInput" class="block text-xs font-bold text-slate-400 uppercase tracking-wide mb-1">Tulis Ulasan (Bahasa Indonesia):</label>
                            <textarea id="sentimentInput" rows="3" class="w-full px-4 py-3 bg-slate-50 dark:bg-slate-900 border border-slate-200 dark:border-slate-700 rounded-xl focus:ring-2 focus:ring-brand-500 focus:outline-none text-sm text-slate-800 dark:text-slate-100" placeholder="Contoh: Bakmie disini enak sekali, kuahnya gurih dan pelayanannya cepat! Tapi porsinya agak sedikit..."></textarea>
                        </div>

                        <!-- Tombol Eksekusi -->
                        <div class="flex justify-between items-center">
                            <div class="flex gap-2">
                                <button onclick="quickReview('positif')" class="text-xs bg-slate-100 dark:bg-slate-700 px-3 py-1.5 rounded-lg hover:bg-emerald-50 dark:hover:bg-emerald-950/50 hover:text-emerald-600 transition">Saran Positif</button>
                                <button onclick="quickReview('negatif')" class="text-xs bg-slate-100 dark:bg-slate-700 px-3 py-1.5 rounded-lg hover:bg-rose-50 dark:hover:bg-rose-950/50 hover:text-rose-600 transition">Saran Negatif</button>
                            </div>
                            <button onclick="analyzeSentiment()" class="inline-flex items-center px-4 py-2 text-sm font-bold text-white bg-indigo-600 hover:bg-indigo-700 rounded-xl transition">
                                Analisis <i class="fa-solid fa-wand-magic-sparkles ml-1.5"></i>
                            </button>
                        </div>

                        <!-- Hasil Sentiment -->
                        <div id="sentimentResult" class="hidden p-4 rounded-2xl border flex items-center gap-4 transition-all duration-300">
                            <!-- Icon Dinamis -->
                            <div id="resultIcon" class="w-12 h-12 rounded-full flex items-center justify-center shrink-0"></div>
                            <!-- Detail Teks -->
                            <div>
                                <span class="text-xs font-bold uppercase tracking-wider block" id="resultLabel">Menunggu...</span>
                                <p class="text-sm text-slate-600 dark:text-slate-400 mt-0.5" id="resultText"></p>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- ALAT 2: SIMULATOR ESTIMASI PENGHEMATAN BIAYA (PROCUREMENT CALCULATOR) -->
                <div class="bg-white dark:bg-slate-800 p-8 rounded-3xl border border-slate-200 dark:border-slate-700 shadow-lg relative overflow-hidden">
                    <span class="absolute top-4 right-4 text-xs font-mono px-2 py-1 rounded bg-emerald-50 dark:bg-emerald-950/50 text-emerald-600 dark:text-emerald-400">
                        Alat Simulasi Bisnis
                    </span>
                    <h3 class="text-xl font-bold text-slate-900 dark:text-white flex items-center gap-2">
                        <i class="fa-solid fa-calculator text-emerald-500"></i> Simulator Efisiensi Biaya (Procurement)
                    </h3>
                    <p class="text-sm text-slate-500 dark:text-slate-400 mt-2">
                        Sebagai staf pengadaan, negosiasi harga satuan dalam volume besar akan menghasilkan penghematan biaya (*Cost Savings*) yang signifikan bagi perusahaan Anda. Uji kalkulator ini untuk melihat perkiraan penghematan yang dinegosiasikan.
                    </p>

                    <div class="mt-6 space-y-4">
                        <div class="grid grid-cols-2 gap-4">
                            <div>
                                <label for="originalPrice" class="block text-xs font-bold text-slate-400 uppercase tracking-wide mb-1">Harga Awal (IDR):</label>
                                <input type="number" id="originalPrice" value="50000" class="w-full px-3 py-2 bg-slate-50 dark:bg-slate-900 border border-slate-200 dark:border-slate-700 rounded-xl text-sm focus:outline-none focus:ring-2 focus:ring-brand-500">
                            </div>
                            <div>
                                <label for="negotiatedPrice" class="block text-xs font-bold text-slate-400 uppercase tracking-wide mb-1">Harga Nego (IDR):</label>
                                <input type="number" id="negotiatedPrice" value="45000" class="w-full px-3 py-2 bg-slate-50 dark:bg-slate-900 border border-slate-200 dark:border-slate-700 rounded-xl text-sm focus:outline-none focus:ring-2 focus:ring-brand-500">
                            </div>
                        </div>
                        <div>
                            <label for="orderQuantity" class="block text-xs font-bold text-slate-400 uppercase tracking-wide mb-1">Volume Kuantitas Pengadaan (Pcs/Kg):</label>
                            <input type="number" id="orderQuantity" value="1000" class="w-full px-3 py-2 bg-slate-50 dark:bg-slate-900 border border-slate-200 dark:border-slate-700 rounded-xl text-sm focus:outline-none focus:ring-2 focus:ring-brand-500">
                        </div>

                        <button onclick="calculateSavings()" class="w-full inline-flex items-center justify-center py-2.5 text-sm font-bold text-white bg-emerald-600 hover:bg-emerald-700 rounded-xl transition">
                            <i class="fa-solid fa-calculator mr-2"></i> Hitung Potensi Penghematan Anggaran
                        </button>

                        <!-- Hasil Kalkulator -->
                        <div id="savingsResult" class="hidden p-4 rounded-2xl bg-emerald-50 dark:bg-emerald-950/20 border border-emerald-100 dark:border-emerald-800/50 flex flex-col sm:flex-row justify-between items-start sm:items-center gap-4">
                            <div>
                                <span class="text-xs text-emerald-600 dark:text-emerald-400 font-bold block">TOTAL ESTIMASI COST SAVING:</span>
                                <span class="text-2xl font-extrabold text-slate-900 dark:text-white" id="savingsValue">IDR 0</span>
                            </div>
                            <div class="px-3 py-1.5 rounded-lg bg-emerald-100 dark:bg-emerald-900/40 text-emerald-700 dark:text-emerald-300 font-bold text-xs" id="savingsPercent">
                                Hemat 0%
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- HUBUNGI SAYA -->
    <section id="kontak" class="py-20 bg-white dark:bg-slate-900/50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <h2 class="text-3xl font-extrabold sm:text-4xl text-slate-900 dark:text-white">Hubungi saya</h2>
                <div class="w-16 h-1 bg-brand-500 mx-auto mt-4 rounded-full"></div>
                <p class="mt-4 text-slate-600 dark:text-slate-400 text-lg">
                    Mari berkolaborasi demi mendorong performa pengadaan perusahaan Anda ke level berikutnya.
                </p>
            </div>

            <div class="grid grid-cols-1 lg:grid-cols-12 gap-12">
                <!-- Kontak Informasi (Kiri - 5 Kolom) -->
                <div class="lg:col-span-5 space-y-6">
                    <h3 class="text-xl font-bold text-slate-900 dark:text-white">Kontak Detail</h3>
                    <p class="text-sm text-slate-500 dark:text-slate-400 leading-relaxed">
                        Jika Anda ingin berdiskusi mengenai proyek pengadaan, integrasi sistem data supply chain, atau menawarkan lowongan karir, jangan ragu untuk menghubungi saya melalui kontak di bawah ini.
                    </p>

                    <div class="space-y-4">
                        <div class="flex items-center gap-4 p-4 bg-slate-50 dark:bg-slate-800 rounded-xl">
                            <div class="w-10 h-10 rounded-lg bg-brand-100 dark:bg-brand-900/40 text-brand-600 dark:text-brand-400 flex items-center justify-center shrink-0">
                                <i class="fa-solid fa-phone"></i>
                            </div>
                            <div>
                                <span class="text-xs text-slate-400 block font-mono">Telepon & WhatsApp</span>
                                <a href="tel:+6281321164034" class="text-sm font-bold text-slate-900 dark:text-white hover:underline">+62 813 2116 4034</a>
                            </div>
                        </div>

                        <div class="flex items-center gap-4 p-4 bg-slate-50 dark:bg-slate-800 rounded-xl">
                            <div class="w-10 h-10 rounded-lg bg-brand-100 dark:bg-brand-900/40 text-brand-600 dark:text-brand-400 flex items-center justify-center shrink-0">
                                <i class="fa-solid fa-envelope"></i>
                            </div>
                            <div>
                                <span class="text-xs text-slate-400 block font-mono">Alamat Email</span>
                                <a href="mailto:julianfarhan12345@gmail.com" class="text-sm font-bold text-slate-900 dark:text-white hover:underline">julianfarhan12345@gmail.com</a>
                            </div>
                        </div>

                        <div class="flex items-center gap-4 p-4 bg-slate-50 dark:bg-slate-800 rounded-xl">
                            <div class="w-10 h-10 rounded-lg bg-brand-100 dark:bg-brand-900/40 text-brand-600 dark:text-brand-400 flex items-center justify-center shrink-0">
                                <i class="fa-brands fa-linkedin-in"></i>
                            </div>
                            <div>
                                <span class="text-xs text-slate-400 block font-mono">LinkedIn Profil</span>
                                <a href="https://linkedin.com/in/julianfarhan/" target="_blank" class="text-sm font-bold text-slate-900 dark:text-white hover:underline">linkedin.com/in/julianfarhan/</a>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Form Kontak (Kanan - 7 Kolom) -->
                <div class="lg:col-span-7">
                    <form id="contactForm" onsubmit="handleContactSubmit(event)" class="space-y-6 bg-slate-50 dark:bg-slate-800 p-8 rounded-3xl border border-slate-200 dark:border-slate-700 shadow-sm">
                        <div class="grid grid-cols-1 sm:grid-cols-2 gap-6">
                            <div>
                                <label for="senderName" class="block text-sm font-semibold text-slate-700 dark:text-slate-300 mb-1">Nama Lengkap</label>
                                <input type="text" id="senderName" required class="w-full px-4 py-2.5 bg-white dark:bg-slate-900 border border-slate-200 dark:border-slate-700 rounded-xl text-sm focus:outline-none focus:ring-2 focus:ring-brand-500">
                            </div>
                            <div>
                                <label for="senderCompany" class="block text-sm font-semibold text-slate-700 dark:text-slate-300 mb-1">Nama Perusahaan</label>
                                <input type="text" id="senderCompany" class="w-full px-4 py-2.5 bg-white dark:bg-slate-900 border border-slate-200 dark:border-slate-700 rounded-xl text-sm focus:outline-none focus:ring-2 focus:ring-brand-500">
                            </div>
                        </div>
                        <div class="grid grid-cols-1 sm:grid-cols-2 gap-6">
                            <div>
                                <label for="senderEmail" class="block text-sm font-semibold text-slate-700 dark:text-slate-300 mb-1">Alamat Email</label>
                                <input type="email" id="senderEmail" required class="w-full px-4 py-2.5 bg-white dark:bg-slate-900 border border-slate-200 dark:border-slate-700 rounded-xl text-sm focus:outline-none focus:ring-2 focus:ring-brand-500">
                            </div>
                            <div>
                                <label for="messageSubject" class="block text-sm font-semibold text-slate-700 dark:text-slate-300 mb-1">Subjek</label>
                                <select id="messageSubject" class="w-full px-4 py-2.5 bg-white dark:bg-slate-900 border border-slate-200 dark:border-slate-700 rounded-xl text-sm focus:outline-none focus:ring-2 focus:ring-brand-500 text-slate-700 dark:text-slate-300">
                                    <option value="Tawaran Kerja">Tawaran Kerja (Fulltime)</option>
                                    <option value="Proyek Freelance">Proyek Konsultasi</option>
                                    <option value="Kerja Sama">Kolaborasi / Lainnya</option>
                                </select>
                            </div>
                        </div>
                        <div>
                            <label for="senderMessage" class="block text-sm font-semibold text-slate-700 dark:text-slate-300 mb-1">Pesan Anda</label>
                            <textarea id="senderMessage" rows="4" required class="w-full px-4 py-2.5 bg-white dark:bg-slate-900 border border-slate-200 dark:border-slate-700 rounded-xl text-sm focus:outline-none focus:ring-2 focus:ring-brand-500" placeholder="Tuliskan detail penawaran kerja sama Anda disini..."></textarea>
                        </div>

                        <button type="submit" class="w-full inline-flex items-center justify-center py-3 text-sm font-bold text-white bg-brand-600 hover:bg-brand-700 rounded-xl transition shadow-lg shadow-brand-500/10">
                            Kirim Pesan <i class="fa-solid fa-paper-plane ml-2"></i>
                        </button>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <!-- FOOTER -->
    <footer class="bg-slate-100 dark:bg-slate-950/80 py-12 border-t border-slate-200 dark:border-slate-800">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex flex-col md:flex-row justify-between items-center gap-6">
                <!-- Slogan & Nama -->
                <div class="text-center md:text-left">
                    <span class="text-lg font-bold bg-gradient-to-r from-brand-600 to-sky-400 bg-clip-text text-transparent">Julian Farhan Wijaya</span>
                    <p class="text-xs text-slate-500 dark:text-slate-400 mt-1">Menggabungkan Efisiensi Pengadaan dan Analitis Data</p>
                </div>

                <!-- Navigasi Footer -->
                <div class="flex flex-wrap justify-center gap-6 text-sm text-slate-500 dark:text-slate-400">
                    <a href="#beranda" class="hover:text-brand-500 transition-colors">Beranda</a>
                    <a href="#tentang" class="hover:text-brand-500 transition-colors">Tentang</a>
                    <a href="#pengalaman" class="hover:text-brand-500 transition-colors">Pengalaman</a>
                    <a href="#keahlian" class="hover:text-brand-500 transition-colors">Keahlian</a>
                    <a href="#proyek" class="hover:text-brand-500 transition-colors">Proyek</a>
                </div>

                <!-- Hak Cipta -->
                <div class="text-xs text-slate-500 dark:text-slate-400">
                    &copy; 2026 JFW. All rights reserved.
                </div>
            </div>
        </div>
    </footer>

    <!-- MODAL CUSTOM UNTUK NOTIFIKASI -->
    <div id="customModal" class="fixed inset-0 z-[100] hidden items-center justify-center p-4 bg-slate-950/60 backdrop-blur-sm">
        <div class="bg-white dark:bg-slate-800 max-w-sm w-full p-6 rounded-2xl border border-slate-200 dark:border-slate-700 shadow-2xl text-center">
            <div id="modalIconContainer" class="w-16 h-16 rounded-full flex items-center justify-center mx-auto mb-4">
                <!-- Icon dimasukkan via JS -->
            </div>
            <h4 id="modalTitle" class="text-lg font-bold text-slate-900 dark:text-white">Judul Modal</h4>
            <p id="modalBody" class="text-sm text-slate-500 dark:text-slate-400 mt-2">Isi pesan dari modal.</p>
            <button onclick="closeModal()" class="mt-6 w-full py-2 bg-brand-600 hover:bg-brand-700 text-white font-bold text-sm rounded-xl transition">
                Selesai
            </button>
        </div>
    </div>

    <!-- JAVASCRIPT UTAMA -->
    <script>
        // DOM Elements
        const themeToggle = document.getElementById('themeToggle');
        const themeIcon = document.getElementById('themeIcon');
        const mobileMenuBtn = document.getElementById('mobileMenuBtn');
        const mobileMenu = document.getElementById('mobileMenu');
        
        // 1. Dark Mode Logic
        if (localStorage.getItem('theme') === 'dark' || (!('theme' in localStorage) && window.matchMedia('(prefers-color-scheme: dark)').matches)) {
            document.documentElement.classList.add('dark');
            themeIcon.className = 'fa-solid fa-sun text-lg';
        } else {
            document.documentElement.classList.remove('dark');
            themeIcon.className = 'fa-solid fa-moon text-lg';
        }

        themeToggle.addEventListener('click', () => {
            if (document.documentElement.classList.contains('dark')) {
                document.documentElement.classList.remove('dark');
                localStorage.setItem('theme', 'light');
                themeIcon.className = 'fa-solid fa-moon text-lg';
            } else {
                document.documentElement.classList.add('dark');
                localStorage.setItem('theme', 'dark');
                themeIcon.className = 'fa-solid fa-sun text-lg';
            }
        });

        // 2. Mobile Menu toggle
        mobileMenuBtn.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });

        // Menutup menu mobile ketika tautan diklik
        mobileMenu.querySelectorAll('a').forEach(link => {
            link.addEventListener('click', () => {
                mobileMenu.classList.add('hidden');
            });
        });

        // 3. Simulator Analisis Sentimen (Berdasarkan Tugas Akhir S1 Informatika)
        function quickReview(tipe) {
            const input = document.getElementById('sentimentInput');
            if (tipe === 'positif') {
                input.value = "Bakmie porsi komplit di warung ini lezat sekali, mienya kenyal dan bumbunya pas. Pelayanan sangat ramah dan tempatnya higienis!";
            } else {
                input.value = "Saya sangat kecewa, pelayanannya lama sekali dan kuah bakmienya dingin saat disajikan. Harganya terlalu mahal untuk rasa yang hambar.";
            }
            analyzeSentiment();
        }

        function analyzeSentiment() {
            const text = document.getElementById('sentimentInput').value.trim().toLowerCase();
            const resultBox = document.getElementById('sentimentResult');
            const resultIcon = document.getElementById('resultIcon');
            const resultLabel = document.getElementById('resultLabel');
            const resultText = document.getElementById('resultText');

            if (!text) {
                showModal("Eror Input", "Harap ketikkan ulasan terlebih dahulu sebelum menekan tombol analisis.", "error");
                return;
            }

            resultBox.classList.remove('hidden');

            // Kata Kunci Sederhana untuk Analisis (Rule-Based Classifier)
            const positiveKeywords = ['enak', 'lezat', 'gurih', 'kenyal', 'mantap', 'ramah', 'cepat', 'murah', 'bersih', 'puas', 'bagus', 'rekomendasi', 'nyaman'];
            const negativeKeywords = ['kecewa', 'lama', 'dingin', 'mahal', 'hambar', 'kotor', 'buruk', 'asin', 'lelet', 'kasar', 'sedikit', 'kurang', 'lambat', 'pelit'];

            let score = 0;
            
            positiveKeywords.forEach(word => {
                if (text.includes(word)) score += 1;
            });
            negativeKeywords.forEach(word => {
                if (text.includes(word)) score -= 1;
            });

            // Update UI dengan hasil analisis
            if (score > 0) {
                resultBox.className = "mt-6 p-4 rounded-2xl border bg-emerald-50 dark:bg-emerald-950/20 border-emerald-100 dark:border-emerald-800/50 flex items-center gap-4 transition-all duration-300";
                resultIcon.className = "w-12 h-12 rounded-full bg-emerald-100 dark:bg-emerald-900/40 text-emerald-600 dark:text-emerald-300 flex items-center justify-center shrink-0 text-xl";
                resultIcon.innerHTML = '<i class="fa-solid fa-face-laugh-beam"></i>';
                resultLabel.className = "text-xs font-bold uppercase tracking-wider block text-emerald-600 dark:text-emerald-400";
                resultLabel.innerText = "SENTIMEN POSITIF (" + score + " poin)";
                resultText.innerText = "Sistem mengklasifikasikan ulasan ini sebagai positif karena mengandung banyak kata pujian. Konsumen puas dengan hidangan Anda!";
            } else if (score < 0) {
                resultBox.className = "mt-6 p-4 rounded-2xl border bg-rose-50 dark:bg-rose-950/20 border-rose-100 dark:border-rose-800/50 flex items-center gap-4 transition-all duration-300";
                resultIcon.className = "w-12 h-12 rounded-full bg-rose-100 dark:bg-rose-900/40 text-rose-600 dark:text-rose-300 flex items-center justify-center shrink-0 text-xl";
                resultIcon.innerHTML = '<i class="fa-solid fa-face-frown"></i>';
                resultLabel.className = "text-xs font-bold uppercase tracking-wider block text-rose-600 dark:text-rose-400";
                resultLabel.innerText = "SENTIMEN NEGATIF (" + Math.abs(score) + " poin)";
                resultText.innerText = "Sistem mengidentifikasi adanya sentimen negatif / keluhan dalam ulasan ini. Menandakan perlu adanya evaluasi kualitas masakan/layanan.";
            } else {
                resultBox.className = "mt-6 p-4 rounded-2xl border bg-slate-50 dark:bg-slate-800 border-slate-200 dark:border-slate-700 flex items-center gap-4 transition-all duration-300";
                resultIcon.className = "w-12 h-12 rounded-full bg-slate-100 dark:bg-slate-700 text-slate-500 dark:text-slate-300 flex items-center justify-center shrink-0 text-xl";
                resultIcon.innerHTML = '<i class="fa-solid fa-face-meh"></i>';
                resultLabel.className = "text-xs font-bold uppercase tracking-wider block text-slate-500 dark:text-slate-400";
                resultLabel.innerText = "SENTIMEN NETRAL (0 poin)";
                resultText.innerText = "Pernyataan berimbang atau tidak memiliki bobot kata emosional yang cukup dominan untuk dikategorikan positif/negatif.";
            }
        }

        // 4. Simulator Kalkulator Procurement (Cost-Saving)
        function calculateSavings() {
            const original = parseFloat(document.getElementById('originalPrice').value);
            const negotiated = parseFloat(document.getElementById('negotiatedPrice').value);
            const qty = parseFloat(document.getElementById('orderQuantity').value);
            const resBox = document.getElementById('savingsResult');
            const valSpan = document.getElementById('savingsValue');
            const pctSpan = document.getElementById('savingsPercent');

            if (isNaN(original) || isNaN(negotiated) || isNaN(qty) || original <= 0 || negotiated <= 0 || qty <= 0) {
                showModal("Eror Input", "Harap lengkapi semua isian kalkulator dengan angka di atas 0.", "error");
                return;
            }

            if (negotiated > original) {
                showModal("Perhatian", "Harga nego lebih besar dari harga awal. Ini akan membebani anggaran perusahaan!", "warning");
            }

            const totalSavings = (original - negotiated) * qty;
            const savingsPercent = ((original - negotiated) / original) * 100;

            // Format rupiah
            const formatted = new Intl.NumberFormat('id-ID', { style: 'currency', currency: 'IDR', maximumFractionDigits: 0 }).format(totalSavings);

            valSpan.innerText = totalSavings >= 0 ? formatted : "-" + formatted.replace("-", "");
            pctSpan.innerText = "Hemat " + savingsPercent.toFixed(1) + "%";

            if (totalSavings >= 0) {
                resBox.className = "hidden sm:flex mt-4 p-4 rounded-2xl bg-emerald-50 dark:bg-emerald-950/20 border border-emerald-100 dark:border-emerald-800/50 justify-between items-center gap-4";
                pctSpan.className = "px-3 py-1.5 rounded-lg bg-emerald-100 dark:bg-emerald-900/40 text-emerald-700 dark:text-emerald-300 font-bold text-xs";
            } else {
                resBox.className = "hidden sm:flex mt-4 p-4 rounded-2xl bg-rose-50 dark:bg-rose-950/20 border border-rose-100 dark:border-rose-800/50 justify-between items-center gap-4";
                pctSpan.className = "px-3 py-1.5 rounded-lg bg-rose-100 dark:bg-rose-900/40 text-rose-700 dark:text-rose-300 font-bold text-xs";
            }
            resBox.classList.remove('hidden');
        }

        // 5. Download Resume Simulator (Menggunakan modifikasi API iFrame Clipboard & file handler)
        function downloadResumeSimulator() {
            showModal("Unduhan CV Dimulai", "Terima kasih atas ketertarikan Anda! Simulasi pengunduhan file 'CV-JULIAN FARHAN WIJAYA.pdf' telah diinisiasi. (Catatan: Ini adalah simulasi responsif portofolio)", "success");
        }

        // 6. Penanganan Kontak & Form Submit
        function handleContactSubmit(event) {
            event.preventDefault();
            const name = document.getElementById('senderName').value;
            const company = document.getElementById('senderCompany').value || "Individu / Umum";
            const email = document.getElementById('senderEmail').value;
            const subject = document.getElementById('messageSubject').value;
            const message = document.getElementById('senderMessage').value;

            // Simulasi sukses kirim pesan
            showModal(
                "Pesan Terkirim!", 
                "Halo " + name + " dari " + company + ", pesan Anda mengenai '" + subject + "' berhasil dikirim secara simulasi. Julian Farhan Wijaya akan segera menghubungi Anda di " + email + ".", 
                "success"
            );
            
            // Bersihkan form
            document.getElementById('contactForm').reset();
        }

        // 7. Modal Kustom (Pengganti alert())
        function showModal(title, body, type = 'success') {
            const modal = document.getElementById('customModal');
            const mTitle = document.getElementById('modalTitle');
            const mBody = document.getElementById('modalBody');
            const mIconContainer = document.getElementById('modalIconContainer');

            mTitle.innerText = title;
            mBody.innerText = body;

            if (type === 'success') {
                mIconContainer.className = "w-16 h-16 rounded-full bg-emerald-100 dark:bg-emerald-900/40 text-emerald-600 dark:text-emerald-300 flex items-center justify-center mx-auto mb-4 text-3xl";
                mIconContainer.innerHTML = '<i class="fa-solid fa-circle-check"></i>';
            } else if (type === 'error') {
                mIconContainer.className = "w-16 h-16 rounded-full bg-rose-100 dark:bg-rose-900/40 text-rose-600 dark:text-rose-300 flex items-center justify-center mx-auto mb-4 text-3xl";
                mIconContainer.innerHTML = '<i class="fa-solid fa-circle-xmark"></i>';
            } else {
                mIconContainer.className = "w-16 h-16 rounded-full bg-amber-100 dark:bg-amber-900/40 text-amber-600 dark:text-amber-300 flex items-center justify-center mx-auto mb-4 text-3xl";
                mIconContainer.innerHTML = '<i class="fa-solid fa-triangle-exclamation"></i>';
            }

            modal.classList.remove('hidden');
            modal.classList.add('flex');
        }

        function closeModal() {
            const modal = document.getElementById('customModal');
            modal.classList.add('hidden');
            modal.classList.remove('flex');
        }
    </script>
</body>
</html>
