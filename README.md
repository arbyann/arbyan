<!DOCTYPE html>
<html lang="id" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Arbyan Nafebri Darmawan - Portofolio TKJ SMKN 1 Surabaya</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Google Fonts: Inter & JetBrains Mono -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&family=JetBrains+Mono:wght@400;500;700&display=swap" rel="stylesheet">
    <!-- Font Awesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

    <script>
        tailwind.config = {
            darkMode: 'class',
            theme: {
                extend: {
                    colors: {
                        cyber: {
                            dark: '#0b0f19',
                            card: '#111827',
                            cardLight: '#1f2937',
                            primary: '#38bdf8',
                            secondary: '#818cf8',
                            accent: '#34d399',
                            glow: 'rgba(56, 189, 248, 0.25)'
                        }
                    },
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                        mono: ['JetBrains Mono', 'monospace']
                    }
                }
            }
        }
    </script>
    <style>
        body {
            background-color: #0b0f19;
            color: #f3f4f6;
            font-family: 'Inter', sans-serif;
            overflow-x: hidden;
        }

        /* Custom Scrollbar */
        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-track {
            background: #0b0f19;
        }
        ::-webkit-scrollbar-thumb {
            background: #1f2937;
            border-radius: 4px;
        }
        ::-webkit-scrollbar-thumb:hover {
            background: #38bdf8;
        }

        /* Background Mesh Grid Pattern */
        .bg-grid-pattern {
            background-size: 40px 40px;
            background-image: 
                linear-gradient(to right, rgba(255, 255, 255, 0.03) 1px, transparent 1px),
                linear-gradient(to bottom, rgba(255, 255, 255, 0.03) 1px, transparent 1px);
        }

        /* Glassmorphism Effect */
        .glass-card {
            background: rgba(17, 24, 39, 0.7);
            backdrop-filter: blur(12px);
            border: 1px solid rgba(255, 255, 255, 0.08);
        }

        .glass-card:hover {
            border-color: rgba(56, 189, 248, 0.4);
            box-shadow: 0 0 25px rgba(56, 189, 248, 0.15);
        }

        /* Gradient Text */
        .gradient-text {
            background: linear-gradient(135deg, #38bdf8 0%, #818cf8 50%, #c084fc 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        /* Pulse Glow Effect */
        @keyframes pulseGlow {
            0%, 100% { opacity: 0.4; transform: scale(1); }
            50% { opacity: 0.8; transform: scale(1.05); }
        }
        .glow-bg {
            animation: pulseGlow 6s infinite ease-in-out;
        }
    </style>
</head>
<body class="bg-grid-pattern relative">

    <!-- Glowing Background Spheres -->
    <div class="fixed top-20 left-10 w-96 h-96 bg-sky-500/10 rounded-full blur-3xl pointer-events-none glow-bg"></div>
    <div class="fixed bottom-20 right-10 w-96 h-96 bg-indigo-500/10 rounded-full blur-3xl pointer-events-none glow-bg" style="animation-delay: -3s;"></div>

    <!-- Navigation Bar -->
    <nav class="fixed top-0 left-0 w-full z-50 glass-card border-b border-gray-800/80 px-6 py-4">
        <div class="max-w-7xl mx-auto flex justify-between items-center">
            <a href="#hero" class="text-xl font-bold font-mono tracking-wider flex items-center gap-2">
                <span class="text-sky-400">&lt;</span>
                <span class="gradient-text font-extrabold">ARBYAN.TKJ</span>
                <span class="text-sky-400">/&gt;</span>
            </a>
            
            <!-- Desktop Menu -->
            <div class="hidden md:flex space-x-8 text-sm font-medium text-gray-300">
                <a href="#about" class="hover:text-sky-400 transition-colors">Tentang Saya</a>
                <a href="#skills" class="hover:text-sky-400 transition-colors">Keahlian</a>
                <a href="#projects" class="hover:text-sky-400 transition-colors">Proyek</a>
                <a href="#timeline" class="hover:text-sky-400 transition-colors">Pendidikan</a>
                <a href="#contact" class="hover:text-sky-400 transition-colors">Kontak</a>
            </div>

            <!-- CTA Header Button -->
            <div class="hidden md:block">
                <a href="#contact" class="px-4 py-2 text-xs font-semibold rounded-lg bg-sky-500/10 text-sky-400 border border-sky-500/30 hover:bg-sky-500 hover:text-gray-900 transition-all duration-300">
                    <i class="fa-solid fa-paper-plane mr-2"></i>Hubungi Saya
                </a>
            </div>

            <!-- Mobile Hamburger Button -->
            <button id="mobile-menu-btn" class="md:hidden text-gray-300 focus:outline-none">
                <i class="fa-solid fa-bars text-xl"></i>
            </button>
        </div>

        <!-- Mobile Menu Modal -->
        <div id="mobile-menu" class="hidden md:hidden pt-4 pb-2 px-2 flex flex-col space-y-3 font-medium text-gray-300">
            <a href="#about" class="hover:text-sky-400 py-1">Tentang Saya</a>
            <a href="#skills" class="hover:text-sky-400 py-1">Keahlian</a>
            <a href="#projects" class="hover:text-sky-400 py-1">Proyek</a>
            <a href="#timeline" class="hover:text-sky-400 py-1">Pendidikan</a>
            <a href="#contact" class="hover:text-sky-400 py-1">Kontak</a>
        </div>
    </nav>

    <!-- SECTION 1: HERO SECTION -->
    <section id="hero" class="min-h-screen flex items-center justify-center pt-28 pb-16 px-6">
        <div class="max-w-7xl mx-auto grid grid-cols-1 lg:grid-cols-12 gap-12 items-center">
            
            <!-- Left Info Column -->
            <div class="lg:col-span-7 space-y-6 text-center lg:text-left">
                <div class="inline-flex items-center gap-2 px-3.5 py-1.5 rounded-full glass-card text-xs text-sky-400 border border-sky-500/20 font-mono">
                    <span class="w-2 h-2 rounded-full bg-emerald-400 animate-ping"></span>
                    <span>Siswa SMKN 1 SURABAYA - Jurusan TKJ</span>
                </div>
                
                <h1 class="text-4xl sm:text-5xl lg:text-6xl font-extrabold tracking-tight leading-tight">
                    Halo, Saya <br class="hidden sm:inline">
                    <span class="gradient-text">ARBYAN NAFEBRI</span> DARMAWAN
                </h1>

                <p class="text-gray-400 text-base sm:text-lg max-w-2xl leading-relaxed">
                    Siswa Teknik Komputer dan Jaringan yang berfokus pada **Infrastruktur Jaringan & Server**, sekaligus secara aktif mempelajari **Bahasa Jepang** demi mewujudkan cita-cita berkarir profesional di Jepang.
                </p>

                <!-- Technical Highlights Badges -->
                <div class="flex flex-wrap justify-center lg:justify-start gap-3 pt-2 font-mono text-xs">
                    <span class="px-3 py-1.5 rounded-md bg-gray-800/80 text-sky-300 border border-gray-700">
                        <i class="fa-solid fa-network-wired text-sky-400 mr-1.5"></i>Teknik Komputer & Jaringan
                    </span>
                    <span class="px-3 py-1.5 rounded-md bg-gray-800/80 text-red-300 border border-gray-700">
                        <i class="fa-solid fa-language text-red-400 mr-1.5"></i>日本語 (Bahasa Jepang)
                    </span>
                    <span class="px-3 py-1.5 rounded-md bg-gray-800/80 text-emerald-300 border border-gray-700">
                        <i class="fa-solid fa-plane-departure text-emerald-400 mr-1.5"></i>Japan Career Aspirant
                    </span>
                </div>

                <!-- Call to Action Buttons -->
                <div class="flex flex-wrap justify-center lg:justify-start gap-4 pt-4">
                    <a href="#about" class="px-6 py-3.5 rounded-xl font-semibold bg-gradient-to-r from-sky-500 to-indigo-600 text-white shadow-lg shadow-sky-500/25 hover:shadow-sky-500/40 hover:scale-[1.02] transition-all">
                        <i class="fa-solid fa-user mr-2"></i>Profil Lengkap
                    </a>
                    <a href="#contact" class="px-6 py-3.5 rounded-xl font-semibold glass-card text-gray-200 hover:text-sky-400 hover:border-sky-500/50 transition-all">
                        <i class="fa-solid fa-envelope mr-2"></i>Hubungi Saya
                    </a>
                </div>
            </div>

            <!-- Right Avatar Column -->
            <div class="lg:col-span-5 flex justify-center">
                <div class="relative w-72 h-72 sm:w-80 sm:h-80 lg:w-96 lg:h-96">
                    <!-- Tech Cyber Ring Accent -->
                    <div class="absolute inset-0 rounded-full border-2 border-dashed border-sky-400/40 animate-[spin_20s_linear_infinite]"></div>
                    <div class="absolute -inset-4 rounded-full border border-indigo-500/20"></div>
                    
                    <!-- Avatar Card Box -->
                    <div class="w-full h-full rounded-3xl glass-card p-4 overflow-hidden relative group flex flex-col justify-between border-2 border-sky-500/30">
                        <div class="absolute inset-0 bg-gradient-to-tr from-sky-500/10 to-indigo-500/10 opacity-50 group-hover:opacity-100 transition-opacity"></div>
                        
                        <!-- Top Terminal Accent Header -->
                        <div class="flex justify-between items-center px-3 py-2 bg-gray-900/80 rounded-xl font-mono text-xs text-gray-400 z-10 border border-gray-800">
                            <div class="flex space-x-1.5">
                                <span class="w-2.5 h-2.5 rounded-full bg-red-500/80"></span>
                                <span class="w-2.5 h-2.5 rounded-full bg-yellow-500/80"></span>
                                <span class="w-2.5 h-2.5 rounded-full bg-green-500/80"></span>
                            </div>
                            <span class="text-sky-400 font-semibold">arbyan@smkn1srb:~</span>
                        </div>

                        <!-- Center Illustration / Avatar Graphic -->
                        <div class="my-auto text-center z-10 py-6">
                            <div class="inline-flex p-6 rounded-full bg-sky-500/10 text-sky-400 border border-sky-500/30 mb-3 shadow-inner">
                                <i class="fa-solid fa-user-gear text-6xl"></i>
                            </div>
                            <h3 class="text-lg font-bold text-white tracking-wide">ARBYAN N. D.</h3>
                            <p class="text-xs text-sky-300 font-mono">TKJ Student • SMKN 1 Surabaya</p>
                        </div>

                        <!-- Bottom Floating Status Card -->
                        <div class="z-10 bg-gray-900/90 rounded-xl p-3 border border-gray-800 text-xs font-mono flex items-center justify-between">
                            <span class="text-gray-400"><i class="fa-solid fa-location-dot text-red-400 mr-1"></i> Surabaya, Indonesia</span>
                            <span class="text-red-400 flex items-center"><i class="fa-solid fa-torii-gate mr-1.5"></i>Target: Japan</span>
                        </div>
                    </div>
                </div>
            </div>

        </div>
    </section>

    <!-- SECTION 2: ABOUT ME SECTION -->
    <section id="about" class="py-20 px-6 relative">
        <div class="max-w-7xl mx-auto">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <h2 class="text-xs font-mono text-sky-400 uppercase tracking-widest mb-2">// Profil Diri</h2>
                <h3 class="text-3xl sm:text-4xl font-bold">Mengenal Lebih Dekat <span class="gradient-text">Arbyan</span></h3>
            </div>

            <div class="glass-card rounded-2xl p-8 max-w-4xl mx-auto border border-gray-800">
                <div class="space-y-4 text-gray-300 leading-relaxed text-sm sm:text-base">
                    <p>
                        Saya adalah siswa jurusan **Teknik Komputer dan Jaringan (TKJ)** di **SMKN 1 Surabaya** yang memiliki minat tinggi pada infrastruktur jaringan, konfigurasi server, serta teknologi informasi terkini.
                    </p>
                    <p>
                        Saat ini, saya juga aktif **mempelajari Bahasa Jepang** secara intensif. Saya memiliki cita-cita dan komitmen yang kuat untuk dapat bekerja di **Jepang** sebagai tenaga profesional di bidang Network & Infrastructure Engineering.
                    </p>
                    <p>
                        Saya percaya bahwa kombinasi antara keahlian teknis TKJ yang solid, disiplin tinggi, serta kemampuan berbahasa Jepang akan menjadi pijakan utama saya untuk berkembang di industri teknologi tingkat internasional.
                    </p>
                </div>

                <div class="mt-8 pt-6 border-t border-gray-800 grid grid-cols-1 sm:grid-cols-3 gap-4 text-center font-mono">
                    <div class="p-3 bg-gray-900/50 rounded-xl border border-gray-800">
                        <span class="block text-xl font-bold text-sky-400">SMKN 1</span>
                        <span class="text-xs text-gray-400">Surabaya</span>
                    </div>
                    <div class="p-3 bg-gray-900/50 rounded-xl border border-gray-800">
                        <span class="block text-xl font-bold text-indigo-400">TKJ</span>
                        <span class="text-xs text-gray-400">Teknik Komputer Jaringan</span>
                    </div>
                    <div class="p-3 bg-gray-900/50 rounded-xl border border-gray-800">
                        <span class="block text-xl font-bold text-emerald-400"><i class="fa-solid fa-torii-gate mr-1"></i> 日本語</span>
                        <span class="text-xs text-gray-400">Persiapan Kerja Jepang</span>
                    </div>
                </div>
            </div>
        </div>
    </section>
    <!-- SECTION 5: EDUCATION TIMELINE -->
    <section id="timeline" class="py-20 px-6 bg-gray-950/50">
        <div class="max-w-4xl mx-auto">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <h2 class="text-xs font-mono text-sky-400 uppercase tracking-widest mb-2">// Jejak Akademik</h2>
                <h3 class="text-3xl sm:text-4xl font-bold">Riwayat <span class="gradient-text">Pendidikan</span></h3>
            </div>

            <div class="relative pl-6 sm:pl-8 border-l-2 border-sky-500/30 space-y-8">
                <!-- Education Item 1: SMKN 1 SURABAYA -->
                <div class="relative group">
                    <div class="absolute -left-[31px] sm:-left-[39px] top-0 w-4 h-4 rounded-full bg-sky-400 border-4 border-gray-950"></div>
                    <div class="glass-card p-6 rounded-2xl border border-gray-800">
                        <span class="text-xs font-mono text-sky-400 font-semibold">2022 - Sekarang</span>
                        <h5 class="text-lg font-bold text-white mt-1">SMKN 1 SURABAYA</h5>
                        <p class="text-xs text-sky-300 font-mono mt-0.5">Jurusan Teknik Komputer dan Jaringan (TKJ)</p>
                        <p class="text-xs text-gray-400 mt-3 leading-relaxed">
                            Mempelajari administrasi server, perancangan arsitektur jaringan LAN/WAN, routing & switching, fiber optic, pengamanan sistem komputer, serta persiapan karir profesional.
                        </p>
                    </div>
                </div>

                <!-- Education Item 2: SMPN 39 SURABAYA -->
                <div class="relative group">
                    <div class="absolute -left-[31px] sm:-left-[39px] top-0 w-4 h-4 rounded-full bg-indigo-400 border-4 border-gray-950"></div>
                    <div class="glass-card p-6 rounded-2xl border border-gray-800">
                        <span class="text-xs font-mono text-indigo-400 font-semibold">Sekolah Menengah Pertama</span>
                        <h5 class="text-lg font-bold text-white mt-1">SMPN 39 SURABAYA</h5>
                        <p class="text-xs text-gray-400 mt-2">
                            Menyelesaikan pendidikan menengah pertama serta aktif mengeksplorasi minat dasar di bidang teknologi informasi dan sains.
                        </p>
                    </div>
                </div>

                <!-- Education Item 3: SDN KALIASIN 1 SURABAYA -->
                <div class="relative group">
                    <div class="absolute -left-[31px] sm:-left-[39px] top-0 w-4 h-4 rounded-full bg-emerald-400 border-4 border-gray-950"></div>
                    <div class="glass-card p-6 rounded-2xl border border-gray-800">
                        <span class="text-xs font-mono text-emerald-400 font-semibold">Sekolah Dasar</span>
                        <h5 class="text-lg font-bold text-white mt-1">SDN KALIASIN 1 SURABAYA</h5>
                        <p class="text-xs text-gray-400 mt-2">
                            Menyelesaikan pendidikan dasar serta membentuk karakter disiplin dan pembiasaan belajar mandiri.
                        </p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- SECTION 7: CONTACT SECTION -->
    <section id="contact" class="py-20 px-6">
        <div class="max-w-7xl mx-auto">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <h2 class="text-xs font-mono text-sky-400 uppercase tracking-widest mb-2">// Jejak Akademik & Sertifikasi</h2>
                <h3 class="text-3xl sm:text-4xl font-bold">Pendidikan & <span class="gradient-text">Pencapaian</span></h3>
            </div>

            <div class="grid grid-cols-1 lg:grid-cols-2 gap-12">
                
                <!-- Education Timeline Column -->
                <div>
                    <h4 class="text-xl font-bold mb-8 flex items-center gap-3 text-sky-400">
                        <i class="fa-solid fa-graduation-cap"></i> Riwayat Pendidikan
                    </h4>

                    <div class="relative pl-6 border-l-2 border-sky-500/30 space-y-8">
                        <!-- Education Item 1 -->
                        <div class="relative group">
                            <div class="absolute -left-[31px] top-0 w-4 h-4 rounded-full bg-sky-400 border-4 border-gray-950"></div>
                            <div class="glass-card p-6 rounded-2xl border border-gray-800">
                                <span class="text-xs font-mono text-sky-400 font-semibold">2022 - Sekarang</span>
                                <h5 class="text-lg font-bold text-white mt-1">SMKN 1 SURABAYA</h5>
                                <p class="text-xs text-sky-300 font-mono mt-0.5">Jurusan Teknik Komputer dan Jaringan (TKJ)</p>
                                <p class="text-xs text-gray-400 mt-3 leading-relaxed">
                                    Fokus pada pembelajaran kompetensi utama: Perancangan Jaringan LAN/WAN, Administrasi Infrastructure Server, Pemeliharaan Jaringan Fiber Optic, dan Keamanan Sistem Komputer.
                                </p>
                            </div>
                        </div>

                        <!-- Education Item 2 -->
                        <div class="relative group">
                            <div class="absolute -left-[31px] top-0 w-4 h-4 rounded-full bg-gray-700 border-4 border-gray-950"></div>
                            <div class="glass-card p-6 rounded-2xl border border-gray-800">
                                <span class="text-xs font-mono text-gray-400">Pendidikan Menengah Pertama</span>
                                <h5 class="text-lg font-bold text-white mt-1">SMP Negeri di Surabaya</h5>
                                <p class="text-xs text-gray-400 mt-2">
                                    Aktif dalam kegiatan ekstrakurikuler sains & teknologi serta dasar-dasar perakitan komputer.
                                </p>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Certifications & Training Column -->
                <div>
                    <h4 class="text-xl font-bold mb-8 flex items-center gap-3 text-indigo-400">
                        <i class="fa-solid fa-certificate"></i> Sertifikasi & Pelatihan
                    </h4>

                    <div class="space-y-4">
                        <!-- Cert 1 -->
                        <div class="glass-card p-5 rounded-2xl border border-gray-800 flex items-start gap-4">
                            <div class="p-3 rounded-xl bg-sky-500/10 text-sky-400 text-xl shrink-0">
                                <i class="fa-solid fa-award"></i>
                            </div>
                            <div>
                                <h5 class="font-bold text-white text-base">Uji Kompetensi Keahlian (UKK) TKJ</h5>
                                <p class="text-xs text-sky-400 font-mono">SMKN 1 Surabaya / BNSP</p>
                                <p class="text-xs text-gray-400 mt-2">
                                    Sertifikasi kompetensi keahlian standar nasional dalam membangun infrastruktur jaringan lokal & internet.
                                </p>
                            </div>
                        </div>

                        <!-- Cert 2 -->
                        <div class="glass-card p-5 rounded-2xl border border-gray-800 flex items-start gap-4">
                            <div class="p-3 rounded-xl bg-indigo-500/10 text-indigo-400 text-xl shrink-0">
                                <i class="fa-solid fa-shield-check"></i>
                            </div>
                            <div>
                                <h5 class="font-bold text-white text-base">MikroTik Certified Network Associate (MTCNA)</h5>
                                <p class="text-xs text-indigo-400 font-mono">MikroTik Academy (Persiapan/Sertifikat)</p>
                                <p class="text-xs text-gray-400 mt-2">
                                    Pemahaman mendalam RouterOS, Routing, Firewall, Wireless, DHCP, DNS, & Quality of Service (QoS).
                                </p>
                            </div>
                        </div>

                        <!-- Cert 3 -->
                        <div class="glass-card p-5 rounded-2xl border border-gray-800 flex items-start gap-4">
                            <div class="p-3 rounded-xl bg-emerald-500/10 text-emerald-400 text-xl shrink-0">
                                <i class="fa-solid fa-graduation-cap"></i>
                            </div>
                            <div>
                                <h5 class="font-bold text-white text-base">Cisco Networking Essentials</h5>
                                <p class="text-xs text-emerald-400 font-mono">Cisco Networking Academy</p>
                                <p class="text-xs text-gray-400 mt-2">
                                    Modul dasar arsitektur komunikasi data, IP Addressing IPv4/IPv6, serta keamanan perangkat keras Cisco.
                                </p>
                            </div>
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- SECTION 6: INTERACTIVE NETWORK UTILITY WIDGET (BONUS FEATURE) -->
    <section id="tools" class="py-20 px-6">
        <div class="max-w-7xl mx-auto">
            <div class="text-center max-w-3xl mx-auto mb-12">
                <h2 class="text-xs font-mono text-sky-400 uppercase tracking-widest mb-2">// Fitur Interaktif</h2>
                <h3 class="text-3xl sm:text-4xl font-bold">Network Tools <span class="gradient-text">Simulator</span></h3>
                <p class="text-gray-400 text-sm mt-3">Fitur interaktif sederhana untuk menghitung Subnet IP IPv4 & mensimulasikan tes ping koneksi jaringan.</p>
            </div>

            <div class="grid grid-cols-1 lg:grid-cols-12 gap-8">
                
                <!-- Tool 1: Subnet Calculator -->
                <div class="lg:col-span-7 glass-card p-6 sm:p-8 rounded-2xl border border-gray-800">
                    <div class="flex items-center gap-3 mb-6">
                        <div class="p-3 rounded-xl bg-sky-500/10 text-sky-400">
                            <i class="fa-solid fa-calculator text-xl"></i>
                        </div>
                        <div>
                            <h4 class="font-bold text-white text-lg">Kalkulator Subnet IPv4</h4>
                            <p class="text-xs text-gray-400">Hitung Subnet Mask & Jumlah Host</p>
                        </div>
                    </div>

                    <div class="grid grid-cols-1 sm:grid-cols-3 gap-4 mb-6">
                        <div class="sm:col-span-2">
                            <label class="block text-xs font-mono text-gray-400 mb-1">IP Address</label>
                            <input type="text" id="ip-input" value="192.168.1.1" class="w-full px-4 py-2.5 rounded-xl bg-gray-900 border border-gray-800 text-white font-mono text-sm focus:outline-none focus:border-sky-500">
                        </div>
                        <div>
                            <label class="block text-xs font-mono text-gray-400 mb-1">Prefix CIDR</label>
                            <select id="cidr-select" class="w-full px-4 py-2.5 rounded-xl bg-gray-900 border border-gray-800 text-white font-mono text-sm focus:outline-none focus:border-sky-500">
                                <option value="24">/24 (255.255.255.0)</option>
                                <option value="25">/25 (255.255.255.128)</option>
                                <option value="26">/26 (255.255.255.192)</option>
                                <option value="27">/27 (255.255.255.224)</option>
                                <option value="28">/28 (255.255.255.240)</option>
                                <option value="29">/29 (255.255.255.248)</option>
                                <option value="30">/30 (255.255.255.252)</option>
                            </select>
                        </div>
                    </div>

                    <button onclick="calculateSubnet()" class="w-full py-3 rounded-xl bg-sky-500 text-gray-900 font-bold text-xs uppercase tracking-wider hover:bg-sky-400 transition-all">
                        Hitung Subnet
                    </button>

                    <!-- Output Box -->
                    <div class="mt-6 p-4 rounded-xl bg-gray-900/90 border border-gray-800 font-mono text-xs space-y-2" id="subnet-result">
                        <div class="flex justify-between border-b border-gray-800 pb-2">
                            <span class="text-gray-400">Subnet Mask:</span>
                            <span class="text-sky-400 font-bold" id="res-mask">255.255.255.0</span>
                        </div>
                        <div class="flex justify-between border-b border-gray-800 pb-2">
                            <span class="text-gray-400">Total Host:</span>
                            <span class="text-indigo-400 font-bold" id="res-hosts">256 IP</span>
                        </div>
                        <div class="flex justify-between border-b border-gray-800 pb-2">
                            <span class="text-gray-400">Usable Host (Valid):</span>
                            <span class="text-emerald-400 font-bold" id="res-usable">254 Host</span>
                        </div>
                        <div class="flex justify-between">
                            <span class="text-gray-400">Wildcard Mask:</span>
                            <span class="text-amber-400 font-bold" id="res-wildcard">0.0.0.255</span>
                        </div>
                    </div>
                </div>

                <!-- Tool 2: Ping Console Simulator -->
                <div class="lg:col-span-5 glass-card p-6 sm:p-8 rounded-2xl border border-gray-800 flex flex-col justify-between">
                    <div>
                        <div class="flex items-center gap-3 mb-6">
                            <div class="p-3 rounded-xl bg-emerald-500/10 text-emerald-400">
                                <i class="fa-solid fa-terminal text-xl"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-white text-lg">Ping Simulator</h4>
                                <p class="text-xs text-gray-400">Tes Responsivitas Latensi Jaringan</p>
                            </div>
                        </div>

                        <div class="flex gap-2 mb-4">
                            <input type="text" id="ping-target" value="smkn1surabaya.sch.id" class="flex-grow px-4 py-2 rounded-xl bg-gray-900 border border-gray-800 text-white font-mono text-xs focus:outline-none focus:border-emerald-500">
                            <button onclick="runPing()" class="px-4 py-2 rounded-xl bg-emerald-500 text-gray-900 font-bold text-xs hover:bg-emerald-400 transition-all">
                                PING
                            </button>
                        </div>

                        <!-- Terminal Output Window -->
                        <div class="h-44 bg-black/90 rounded-xl p-3 font-mono text-[11px] text-emerald-400 overflow-y-auto border border-gray-800" id="ping-output">
                            <p class="text-gray-500">// Masukkan host dan tekan PING...</p>
                        </div>
                    </div>

                    <div class="mt-4 text-[10px] font-mono text-gray-500 text-center">
                        Simulasi CLI ICMP Packets
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- SECTION 7: CONTACT SECTION -->
    <section id="contact" class="py-20 px-6 bg-gray-950/50">
        <div class="max-w-7xl mx-auto">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <h2 class="text-xs font-mono text-sky-400 uppercase tracking-widest mb-2">// Mari Terhubung</h2>
                <h3 class="text-3xl sm:text-4xl font-bold">Kontak <span class="gradient-text">Arbyan</span></h3>
                <p class="text-gray-400 text-sm mt-3">Apakah Anda ingin berdiskusi seputar proyek jaringan, kolaborasi, atau peluang magang/PKL?</p>
            </div>

            <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 items-start">
                
                <!-- Social Links & Info Column -->
                <div class="lg:col-span-5 space-y-6">
                    <div class="glass-card p-6 rounded-2xl border border-gray-800 space-y-6">
                        <div class="flex items-center gap-4">
                            <div class="w-12 h-12 rounded-xl bg-sky-500/10 text-sky-400 flex items-center justify-center text-xl shrink-0">
                                <i class="fa-solid fa-envelope"></i>
                            </div>
                            <div>
                                <span class="text-xs text-gray-400 block font-mono">Email Resmi</span>
                                <a href="mailto:arbyan.nafebri@gmail.com" class="text-sm font-semibold text-white hover:text-sky-400 transition-colors">arbyan.nafebri@gmail.com</a>
                            </div>
                        </div>

                        <div class="flex items-center gap-4">
                            <div class="w-12 h-12 rounded-xl bg-emerald-500/10 text-emerald-400 flex items-center justify-center text-xl shrink-0">
                                <i class="fa-brands fa-whatsapp"></i>
                            </div>
                            <div>
                                <span class="text-xs text-gray-400 block font-mono">WhatsApp</span>
                                <a href="https://wa.me/628123456789" target="_blank" class="text-sm font-semibold text-white hover:text-emerald-400 transition-colors">+62 812-xxxx-xxxx</a>
                            </div>
                        </div>

                        <div class="flex items-center gap-4">
                            <div class="w-12 h-12 rounded-xl bg-indigo-500/10 text-indigo-400 flex items-center justify-center text-xl shrink-0">
                                <i class="fa-solid fa-location-dot"></i>
                            </div>
                            <div>
                                <span class="text-xs text-gray-400 block font-mono">Lokasi Sekolah / Domisili</span>
                                <span class="text-sm font-semibold text-white">Surabaya, Jawa Timur, Indonesia</span>
                            </div>
                        </div>
                    </div>

                    <!-- Social Icons Row -->
                    <div class="glass-card p-6 rounded-2xl border border-gray-800 text-center">
                        <span class="text-xs text-gray-400 font-mono block mb-4">Media Sosial & Portofolio Kode</span>
                        <div class="flex justify-center gap-4 text-lg">
                            <a href="#" class="w-10 h-10 rounded-xl bg-gray-800 text-gray-300 hover:text-sky-400 hover:bg-gray-700 flex items-center justify-center transition-all"><i class="fa-brands fa-linkedin-in"></i></a>
                            <a href="#" class="w-10 h-10 rounded-xl bg-gray-800 text-gray-300 hover:text-white hover:bg-gray-700 flex items-center justify-center transition-all"><i class="fa-brands fa-github"></i></a>
                            <a href="#" class="w-10 h-10 rounded-xl bg-gray-800 text-gray-300 hover:text-pink-400 hover:bg-gray-700 flex items-center justify-center transition-all"><i class="fa-brands fa-instagram"></i></a>
                        </div>
                    </div>
                </div>

                <!-- Glassmorphism Contact Form Column -->
                <div class="lg:col-span-7 glass-card p-8 rounded-2xl border border-gray-800">
                    <form id="contact-form" onsubmit="handleFormSubmit(event)" class="space-y-6">
                        <div class="grid grid-cols-1 sm:grid-cols-2 gap-6">
                            <div>
                                <label class="block text-xs font-mono text-gray-400 mb-2">Nama Lengkap</label>
                                <input type="text" required placeholder="Masukkan nama Anda" class="w-full px-4 py-3 rounded-xl bg-gray-900 border border-gray-800 text-white text-sm focus:outline-none focus:border-sky-500 transition-colors">
                            </div>
                            <div>
                                <label class="block text-xs font-mono text-gray-400 mb-2">Alamat Email</label>
                                <input type="email" required placeholder="nama@email.com" class="w-full px-4 py-3 rounded-xl bg-gray-900 border border-gray-800 text-white text-sm focus:outline-none focus:border-sky-500 transition-colors">
                            </div>
                        </div>

                        <div>
                            <label class="block text-xs font-mono text-gray-400 mb-2">Subjek Pesan</label>
                            <input type="text" required placeholder="Contoh: Penawaran PKL / Diskusi Jaringan" class="w-full px-4 py-3 rounded-xl bg-gray-900 border border-gray-800 text-white text-sm focus:outline-none focus:border-sky-500 transition-colors">
                        </div>

                        <div>
                            <label class="block text-xs font-mono text-gray-400 mb-2">Pesan Anda</label>
                            <textarea rows="4" required placeholder="Tuliskan pesan Anda secara rinci..." class="w-full px-4 py-3 rounded-xl bg-gray-900 border border-gray-800 text-white text-sm focus:outline-none focus:border-sky-500 transition-colors"></textarea>
                        </div>

                        <button type="submit" class="w-full py-3.5 rounded-xl bg-gradient-to-r from-sky-500 to-indigo-600 text-white font-bold text-sm shadow-lg shadow-sky-500/20 hover:shadow-sky-500/40 transition-all flex items-center justify-center gap-2">
                            <i class="fa-solid fa-paper-plane"></i> Kirim Pesan Sekarang
                        </button>
                    </form>
                    
                    <!-- Form Status Message Alert -->
                    <div id="form-alert" class="hidden mt-4 p-4 rounded-xl text-xs font-mono text-center"></div>
                </div>

            </div>
        </div>
    </section>

    <!-- FOOTER -->
    <footer class="py-8 px-6 border-t border-gray-800 text-center text-xs text-gray-500 font-mono">
        <div class="max-w-7xl mx-auto flex flex-col sm:flex-row justify-between items-center gap-4">
            <div>
                © 2026 <span class="text-sky-400 font-bold">Arbyan Nafebri Darmawan</span>. SMKN 1 Surabaya (TKJ).
            </div>
            <div>
                Built with HTML5, Tailwind CSS & JavaScript
            </div>
        </div>
    </footer>

    <!-- JAVASCRIPT LOGIC -->
    <script>
        // Mobile Navigation Menu Toggle
        const mobileMenuBtn = document.getElementById('mobile-menu-btn');
        const mobileMenu = document.getElementById('mobile-menu');

        mobileMenuBtn.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });

        // Close mobile menu on link click
        document.querySelectorAll('#mobile-menu a').forEach(link => {
            link.addEventListener('click', () => {
                mobileMenu.classList.add('hidden');
            });
        });

        // Project Filter Logic
        const filterBtns = document.querySelectorAll('.filter-btn');
        const projectCards = document.querySelectorAll('.project-card');

        filterBtns.forEach(btn => {
            btn.addEventListener('click', () => {
                filterBtns.forEach(b => {
                    b.classList.remove('bg-sky-500', 'text-gray-900');
                    b.classList.add('glass-card', 'text-gray-300');
                });
                
                btn.classList.add('bg-sky-500', 'text-gray-900');
                btn.classList.remove('glass-card', 'text-gray-300');

                const filter = btn.getAttribute('data-filter');

                projectCards.forEach(card => {
                    if (filter === 'all' || card.getAttribute('data-category') === filter) {
                        card.style.display = 'block';
                    } else {
                        card.style.display = 'none';
                    }
                });
            });
        });

        // Project Modal Popups Data
        const projectsData = {
            project1: {
                title: 'Manajemen Bandwidth & Hotspot Sekolah',
                category: 'MikroTik RouterOS',
                description: 'Proyek ini berfokus pada implementasi manajemen alokasi bandwidth bagi para siswa dan guru di lingkungan sekolah menggunakan RouterBoard MikroTik RB750r2.',
                details: [
                    'Menerapkan Queue Tree untuk pembagian alokasi bertingkat.',
                    'Membuat Portal Hotspot kustom dengan autentikasi User Manager.',
                    'Melakukan filtering situs tidak aman melalui Layer 7 Protocol Firewall.'
                ],
                tech: ['MikroTik RouterOS', 'Winbox', 'Queue Tree', 'Firewall Filter']
            },
            project2: {
                title: 'Deployment Server Infrastructure Lokal',
                category: 'Linux Debian 11',
                description: 'Membangun infrastruktur server lokal lengkap di sistem Linux Debian 11 untuk mendukung kebutuhan aplikasi berbasis web dan resolusi nama domain lokal.',
                details: [
                    'Konfigurasi Bind9 DNS Server dengan Zone Forwarder & Reverse.',
                    'Instalasi Web Server Apache2, PHP, & database MySQL.',
                    'Penyetelan ISC-DHCP-Server untuk alokasi IP otomatis ke klien.'
                ],
                tech: ['Debian Server', 'Apache2', 'MySQL', 'Bind9 DNS', 'DHCP']
            },
            project3: {
                title: 'Desain Topologi Multi-VLAN Inter-VLAN Routing',
                category: 'Cisco Packet Tracer',
                description: 'Perancangan simulasi topologi jaringan enterprise terintegrasi dengan segmentasi trafik lalu lintas jaringan antar divisi gedung.',
                details: [
                    'Konfigurasi VLAN Trunking Protocol (VTP) dan 802.1Q.',
                    'Implementasi Router-on-a-Stick untuk komunikasi Inter-VLAN.',
                    'Konfigurasi OSPF Routing Protocol untuk skalabilitas rute.'
                ],
                tech: ['Cisco Packet Tracer', 'VLAN', 'Inter-VLAN', 'OSPF']
            },
            project4: {
                title: 'Penyambungan Kabel Fiber Optic & Pengukuran OPM',
                category: 'Fiber Optic Physical Layer',
                description: 'Pekerjaan praktikum lapangan mencakup pengupasan, pembersihan, splicing core serat optik, hingga verifikasi nilai desibel loss.',
                details: [
                    'Penyambungan core serat optik menggunakan Fusion Splicer.',
                    'Pengujian nilai dBm redaman kabel menggunakan Optical Power Meter (OPM).',
                    'Crimping Fast Connector SC/UPC untuk terminasi pigtail.'
                ],
                tech: ['Fusion Splicer', 'OPM', 'Cleaver', 'Fiber Core']
            },
            project5: {
                title: 'Virtualisasi Server dengan Proxmox VE',
                category: 'Virtualization & Cloud',
                description: 'Penggunaan Proxmox VE (Virtual Environment) untuk mengoptimalkan penggunaan resource hardware fisik server sekolah.',
                details: [
                    'Instalasi Proxmox VE Hypervisor pada Bare-Metal Hardware.',
                    'Membuat Container (LXC) ringan untuk Web Server dan Storage.',
                    'Penyetelan Network Bridge untuk komunikasi VM internal/eksternal.'
                ],
                tech: ['Proxmox VE', 'Virtualization', 'LXC Container', 'Bridge Networking']
            }
        };

        function openModal(projectId) {
            const data = projectsData[projectId];
            if (!data) return;

            const modalContent = document.getElementById('modal-content');
            modalContent.innerHTML = `
                <span class="px-3 py-1 rounded-full text-[10px] font-mono bg-sky-500/20 text-sky-400 border border-sky-500/30 font-semibold">${data.category}</span>
                <h3 class="text-2xl font-bold text-white mt-3 mb-4">${data.title}</h3>
                <p class="text-sm text-gray-300 leading-relaxed mb-6">${data.description}</p>
                
                <h4 class="text-xs font-mono text-sky-400 uppercase tracking-wider mb-2">Poin Penting Pengerjaan:</h4>
                <ul class="list-disc list-inside space-y-2 text-xs text-gray-400 mb-6">
                    ${data.details.map(d => `<li>${d}</li>`).join('')}
                </ul>

                <h4 class="text-xs font-mono text-sky-400 uppercase tracking-wider mb-2">Teknologi Digunakan:</h4>
                <div class="flex flex-wrap gap-2 font-mono text-xs">
                    ${data.tech.map(t => `<span class="px-2.5 py-1 rounded-md bg-gray-800 text-gray-200 border border-gray-700">${t}</span>`).join('')}
                </div>
            `;

            document.getElementById('project-modal').classList.remove('hidden');
        }

        function closeModal() {
            document.getElementById('project-modal').classList.add('hidden');
        }

        // Close modal on outside click
        document.getElementById('project-modal').addEventListener('click', (e) => {
            if (e.target === document.getElementById('project-modal')) {
                closeModal();
            }
        });

        // Contact Form Handler
        function handleFormSubmit(e) {
            e.preventDefault();
            const alertBox = document.getElementById('form-alert');
            alertBox.classList.remove('hidden', 'bg-red-500/20', 'text-red-400');
            alertBox.classList.add('bg-emerald-500/20', 'text-emerald-400', 'border', 'border-emerald-500/30');
            alertBox.innerText = "Terima kasih! Pesan Anda telah berhasil dikirimkan ke Arbyan.";
            
            document.getElementById('contact-form').reset();
            setTimeout(() => {
                alertBox.classList.add('hidden');
            }, 5000);
        }
    </script>
</body>
</html>
