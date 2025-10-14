<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>EcoAndGold - Sinergi Aset Lahan, Bisnis, dan Mineral Indonesia</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;500;600;700&family=Playfair+Display:wght@400;500;600;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary-black: #1a1a1a;
            --secondary-gray: #4a4a4a;
            --light-gray: #f5f5f5;
            --gold: #D4AF37;
            --white: #ffffff;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Montserrat', sans-serif;
            line-height: 1.6;
            color: var(--primary-black);
            background-color: var(--white);
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* Header Styles */
        header {
            background-color: var(--white);
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
        }
        
        .nav-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1rem 0;
        }
        
        .logo {
            font-family: 'Playfair Display', serif;
            font-size: 1.8rem;
            font-weight: 700;
            color: var(--primary-black);
            text-decoration: none;
        }
        
        .logo span {
            color: var(--gold);
        }
        
        /* Language Selector */
        .language-selector {
            position: relative;
            display: inline-block;
        }
        
        .language-btn {
            background: var(--light-gray);
            border: 2px solid #e0e0e0;
            padding: 8px 15px;
            border-radius: 5px;
            cursor: pointer;
            display: flex;
            align-items: center;
            gap: 8px;
            font-weight: 500;
            transition: all 0.3s;
        }
        
        .language-btn:hover {
            border-color: var(--gold);
        }
        
        .language-btn img {
            width: 20px;
            height: 15px;
            object-fit: cover;
        }
        
        .language-dropdown {
            display: none;
            position: absolute;
            top: 100%;
            right: 0;
            background: var(--white);
            min-width: 150px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            border-radius: 5px;
            overflow: hidden;
            z-index: 1001;
        }
        
        .language-dropdown.show {
            display: block;
        }
        
        .language-option {
            padding: 12px 15px;
            cursor: pointer;
            display: flex;
            align-items: center;
            gap: 10px;
            transition: background-color 0.3s;
            border-bottom: 1px solid #f0f0f0;
        }
        
        .language-option:hover {
            background-color: var(--light-gray);
        }
        
        .language-option:last-child {
            border-bottom: none;
        }
        
        .language-option img {
            width: 20px;
            height: 15px;
            object-fit: cover;
        }
        
        .language-option.active {
            background-color: var(--gold);
            color: var(--white);
        }
        
        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, var(--light-gray) 0%, var(--white) 100%);
            padding: 120px 0 80px;
            text-align: center;
        }
        
        .hero h1 {
            font-family: 'Playfair Display', serif;
            font-size: 3rem;
            font-weight: 700;
            margin-bottom: 1rem;
            color: var(--primary-black);
        }
        
        .hero p {
            font-size: 1.2rem;
            color: var(--secondary-gray);
            max-width: 600px;
            margin: 0 auto 2rem;
        }
        
        /* Search Form */
        .search-form {
            max-width: 500px;
            margin: 0 auto;
            display: flex;
            gap: 10px;
        }
        
        .search-input {
            flex: 1;
            padding: 15px 20px;
            border: 2px solid #e0e0e0;
            border-radius: 5px;
            font-size: 1rem;
            transition: border-color 0.3s;
        }
        
        .search-input:focus {
            outline: none;
            border-color: var(--gold);
        }
        
        .search-btn {
            background-color: var(--gold);
            color: var(--white);
            border: none;
            padding: 15px 30px;
            border-radius: 5px;
            font-weight: 600;
            cursor: pointer;
            transition: background-color 0.3s;
        }
        
        .search-btn:hover {
            background-color: #b8941f;
        }
        
        /* Business Model Section */
        .business-model {
            padding: 80px 0;
            background-color: var(--white);
        }
        
        .model-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin-top: 3rem;
        }
        
        .model-card {
            background: var(--light-gray);
            padding: 40px 30px;
            border-radius: 10px;
            text-align: center;
            transition: transform 0.3s;
            border-left: 4px solid var(--gold);
        }
        
        .model-card:hover {
            transform: translateY(-5px);
        }
        
        .model-icon {
            font-size: 3rem;
            margin-bottom: 1rem;
        }
        
        .model-card h3 {
            color: var(--primary-black);
            margin-bottom: 1rem;
            font-size: 1.5rem;
        }
        
        /* About Section */
        .about {
            padding: 80px 0;
            background-color: var(--light-gray);
        }
        
        .about-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 50px;
            align-items: center;
        }
        
        .about-text h2 {
            font-family: 'Playfair Display', serif;
            font-size: 2.5rem;
            margin-bottom: 1.5rem;
            color: var(--primary-black);
        }
        
        .about-text p {
            color: var(--secondary-gray);
            margin-bottom: 1.5rem;
        }
        
        /* Contact Form Section */
        .contact {
            padding: 80px 0;
            background-color: var(--white);
        }
        
        .contact-form {
            max-width: 600px;
            margin: 0 auto;
            background: var(--light-gray);
            padding: 40px;
            border-radius: 10px;
        }
        
        .form-group {
            margin-bottom: 20px;
        }
        
        .form-group label {
            display: block;
            margin-bottom: 5px;
            font-weight: 600;
            color: var(--primary-black);
        }
        
        .form-group input,
        .form-group textarea,
        .form-group select {
            width: 100%;
            padding: 12px 15px;
            border: 2px solid #e0e0e0;
            border-radius: 5px;
            font-size: 1rem;
            transition: border-color 0.3s;
        }
        
        .form-group input:focus,
        .form-group textarea:focus,
        .form-group select:focus {
            outline: none;
            border-color: var(--gold);
        }
        
        .form-row {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 15px;
        }
        
        .submit-btn {
            background-color: var(--gold);
            color: var(--white);
            border: none;
            padding: 15px 40px;
            border-radius: 5px;
            font-weight: 600;
            cursor: pointer;
            transition: background-color 0.3s;
            width: 100%;
            font-size: 1.1rem;
        }
        
        .submit-btn:hover {
            background-color: #b8941f;
        }
        
        /* Impact Section */
        .impact {
            padding: 80px 0;
            background-color: var(--primary-black);
            color: var(--white);
        }
        
        .impact-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
            margin-top: 3rem;
        }
        
        .impact-item {
            text-align: center;
            padding: 30px;
        }
        
        .impact-number {
            font-size: 3rem;
            font-weight: 700;
            color: var(--gold);
            margin-bottom: 1rem;
        }
        
        /* Footer */
        footer {
            background-color: var(--primary-black);
            color: var(--white);
            padding: 40px 0;
            text-align: center;
        }
        
        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 30px;
            margin-bottom: 2rem;
        }
        
        .footer-section h3 {
            color: var(--gold);
            margin-bottom: 1rem;
        }
        
        .copyright {
            border-top: 1px solid #333;
            padding-top: 2rem;
            opacity: 0.7;
        }
        
        .section-title {
            text-align: center;
            font-family: 'Playfair Display', serif;
            font-size: 2.5rem;
            margin-bottom: 3rem;
            color: var(--primary-black);
        }
        
        .impact .section-title {
            color: var(--white);
        }
        
        /* Responsive Design */
        @media (max-width: 768px) {
            .about-content {
                grid-template-columns: 1fr;
            }
            
            .form-row {
                grid-template-columns: 1fr;
            }
            
            .hero h1 {
                font-size: 2rem;
            }
            
            .search-form {
                flex-direction: column;
            }
            
            .contact-form {
                padding: 20px;
            }
            
            .nav-container {
                flex-direction: column;
                gap: 15px;
            }
            
            .language-selector {
                align-self: flex-end;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container">
            <nav class="nav-container">
                <a href="#" class="logo">ECOAND<span>GOLD</span></a>
                <div class="language-selector">
                    <button class="language-btn" id="languageBtn">
                        <img src="https://flagcdn.com/w20/id.png" alt="Indonesian Flag">
                        <span>Indonesia</span>
                        <span>▼</span>
                    </button>
                    <div class="language-dropdown" id="languageDropdown">
                        <div class="language-option active" data-lang="id">
                            <img src="https://flagcdn.com/w20/id.png" alt="Indonesian Flag">
                            <span>Indonesia</span>
                        </div>
                        <div class="language-option" data-lang="en">
                            <img src="https://flagcdn.com/w20/us.png" alt="USA Flag">
                            <span>English</span>
                        </div>
                        <div class="language-option" data-lang="cn">
                            <img src="https://flagcdn.com/w20/cn.png" alt="China Flag">
                            <span>中文</span>
                        </div>
                        <div class="language-option" data-lang="jp">
                            <img src="https://flagcdn.com/w20/jp.png" alt="Japan Flag">
                            <span>日本語</span>
                        </div>
                        <div class="language-option" data-lang="kr">
                            <img src="https://flagcdn.com/w20/kr.png" alt="South Korea Flag">
                            <span>한국어</span>
                        </div>
                    </div>
                </div>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <div class="container">
            <h1>Sinergi Aset Lahan, Bisnis, dan Mineral Indonesia</h1>
            <p>Menghubungkan potensi lahan, mengembangkan bisnis berkelanjutan, dan mengoptimalkan kekayaan mineral Indonesia untuk pasar global</p>
            
            <form class="search-form" id="productSearchForm">
                <input type="text" class="search-input" placeholder="Jenis mineral atau komoditas yang Anda butuhkan..." required>
                <button type="submit" class="search-btn">Cari Produk</button>
            </form>
        </div>
    </section>

    <!-- Business Model Section -->
    <section class="business-model">
        <div class="container">
            <h2 class="section-title">Tiga Pilar Utama Kami</h2>
            <div class="model-grid">
                <div class="model-card">
                    <div class="model-icon">🏞️</div>
                    <h3>Aset Lahan</h3>
                    <p>Pengelolaan lahan strategis yang kaya akan sumber daya mineral dengan pendekatan berkelanjutan dan ramah lingkungan</p>
                </div>
                <div class="model-card">
                    <div class="model-icon">💼</div>
                    <h3>Pengembangan Bisnis</h3>
                    <p>Membangun model bisnis yang profitable dan sustainable dari hulu hingga hilir</p>
                </div>
                <div class="model-card">
                    <div class="model-icon">💎</div>
                    <h3>Mineral Berharga</h3>
                    <p>Eksplorasi dan ekspor mineral bernilai tinggi dengan standar kualitas internasional</p>
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section class="about">
        <div class="container">
            <div class="about-content">
                <div class="about-text">
                    <h2>Visi Kami</h2>
                    <p>EcoAndGold menghadirkan integrasi antara <strong>aset lahan</strong> yang strategis, <strong>pengembangan bisnis</strong> yang berkelanjutan, dan <strong>potensi mineral</strong> berkualitas tinggi dari berbagai wilayah di Indonesia.</p>
                    <p>Dengan fokus pada ekspor dan pemenuhan kebutuhan dalam negeri, kami berkomitmen untuk memberikan kontribusi signifikan bagi perekonomian lokal dan nasional.</p>
                </div>
                <div class="about-image">
                    <div style="background-color: var(--white); height: 400px; border-radius: 5px; display: flex; align-items: center; justify-content: center; color: var(--secondary-gray); border: 2px dashed #ddd;">
                        [Gambar Peta Lokasi Lahan atau Operasional]
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Form Section -->
    <section class="contact">
        <div class="container">
            <h2 class="section-title">Hubungi Kami Segera</h2>
            <div class="contact-form">
                <form id="contactForm">
                    <div class="form-row">
                        <div class="form-group">
                            <label for="name">Nama Lengkap *</label>
                            <input type="text" id="name" name="name" required>
                        </div>
                        <div class="form-group">
                            <label for="company">Perusahaan</label>
                            <input type="text" id="company" name="company">
                        </div>
                    </div>
                    
                    <div class="form-row">
                        <div class="form-group">
                            <label for="email">Email *</label>
                            <input type="email" id="email" name="email" required>
                        </div>
                        <div class="form-group">
                            <label for="phone">Nomor Telepon *</label>
                            <input type="tel" id="phone" name="phone" required placeholder="+62 xxx xxxx xxxx">
                        </div>
                    </div>
                    
                    <div class="form-group">
                        <label for="interest">Minat Terkait</label>
                        <select id="interest" name="interest">
                            <option value="">Pilih minat Anda</option>
                            <option value="lahan">Kerjasama Pengelolaan Lahan</option>
                            <option value="bisnis">Peluang Bisnis</option>
                            <option value="mineral">Pembelian Mineral</option>
                            <option value="ekspor">Kerjasama Ekspor</option>
                            <option value="lainnya">Lainnya</option>
                        </select>
                    </div>
                    
                    <div class="form-group">
                        <label for="product">Produk/Mineral yang Dicari</label>
                        <input type="text" id="product" name="product" placeholder="Jenis mineral atau komoditas yang dibutuhkan">
                    </div>
                    
                    <div class="form-group">
                        <label for="message">Pesan *</label>
                        <textarea id="message" name="message" rows="5" required placeholder="Jelaskan kebutuhan atau pertanyaan Anda..."></textarea>
                    </div>
                    
                    <button type="submit" class="submit-btn">Kirim Pesan</button>
                </form>
            </div>
        </div>
    </section>

    <!-- Impact Section -->
    <section class="impact">
        <div class="container">
            <h2 class="section-title">Dampak Positif Kami</h2>
            <div class="impact-grid">
                <div class="impact-item">
                    <div class="impact-number">100+</div>
                    <h3>Hektar Lahan Terkelola</h3>
                    <p>Pengelolaan lahan berkelanjutan di berbagai wilayah Indonesia</p>
                </div>
                <div class="impact-item">
                    <div class="impact-number">50+</div>
                    <h3>Mitra Bisnis</h3>
                    <p>Jaringan mitra lokal dan internasional yang kuat</p>
                </div>
                <div class="impact-item">
                    <div class="impact-number">10+</div>
                    <h3>Jenis Mineral</h3>
                    <p>Beragam mineral berkualitas untuk berbagai industri</p>
                </div>
                <div class="impact-item">
                    <div class="impact-number">5+</div>
                    <h3>Negara Tujuan Ekspor</h3>
                    <p>Jangkauan pasar internasional yang terus berkembang</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-section">
                    <h3>EcoAndGold</h3>
                    <p>Integrator terpercaya untuk pengelolaan lahan, pengembangan bisnis, dan perdagangan mineral Indonesia.</p>
                </div>
                <div class="footer-section">
                    <h3>Kontak Cepat</h3>
                    <p>📧 info@ecoandgold.com</p>
                    <p>📞 +62 XXX XXXX XXXX</p>
                    <p>📍 Beroperasi di seluruh Indonesia</p>
                </div>
                <div class="footer-section">
                    <h3>Fokus Kami</h3>
                    <p>• Aset Lahan</p>
                    <p>• Pengembangan Bisnis</p>
                    <p>• Mineral Berharga</p>
                    <p>• Ekspor & Domestik</p>
                </div>
            </div>
            <div class="copyright">
                <p>&copy; 2024 EcoAndGold. All rights reserved. | Sinergi untuk Indonesia yang Lebih Baik</p>
            </div>
        </div>
    </footer>

    <script>
        // Language Selector Functionality
        const languageBtn = document.getElementById('languageBtn');
        const languageDropdown = document.getElementById('languageDropdown');
        const languageOptions = document.querySelectorAll('.language-option');

        // Toggle dropdown
        languageBtn.addEventListener('click', function(e) {
            e.stopPropagation();
            languageDropdown.classList.toggle('show');
        });

        // Close dropdown when clicking outside
        document.addEventListener('click', function() {
            languageDropdown.classList.remove('show');
        });

        // Language selection
        languageOptions.forEach(option => {
            option.addEventListener('click', function() {
                const selectedLang = this.getAttribute('data-lang');
                
                // Update active state
                languageOptions.forEach(opt => opt.classList.remove('active'));
                this.classList.add('active');
                
                // Update button text and flag
                const flagSrc = this.querySelector('img').src;
                const languageText = this.querySelector('span').textContent;
                
                languageBtn.querySelector('img').src = flagSrc;
                languageBtn.querySelector('span').textContent = languageText;
                
                // Close dropdown
                languageDropdown.classList.remove('show');
                
                // Here you would typically load the translation for the selected language
                changeLanguage(selectedLang);
            });
        });

        // Function to change language (placeholder for actual translation)
        function changeLanguage(lang) {
            // This is where you would implement actual translation
            // For now, we'll just show an alert
            const languages = {
                'id': 'Indonesia',
                'en': 'English',
                'cn': 'Chinese',
                'jp': 'Japanese',
                'kr': 'Korean'
            };
            
            alert(`Language changed to ${languages[lang]}. Actual translation would be implemented here.`);
            
            // Example of what actual implementation would look like:
            // fetch(`translations/${lang}.json`)
            //     .then(response => response.json())
            //     .then(translations => {
            //         document.querySelectorAll('[data-translate]').forEach(element => {
            //             const key = element.getAttribute('data-translate');
            //             element.textContent = translations[key];
            //         });
            //     });
        }

        // Form handling untuk pencarian produk
        document.getElementById('productSearchForm').addEventListener('submit', function(e) {
            e.preventDefault();
            const productName = this.querySelector('.search-input').value;
            alert(`Terima kasih! Permintaan untuk "${productName}" telah kami terima. Tim kami akan menghubungi Anda dalam 1x24 jam.`);
            this.reset();
        });

        // Form handling untuk kontak
        document.getElementById('contactForm').addEventListener('submit', function(e) {
            e.preventDefault();
            
            // Ambil data form
            const name = document.getElementById('name').value;
            const phone = document.getElementById('phone').value;
            const product = document.getElementById('product').value;
            
            alert(`Terima kasih ${name}! Pesan Anda telah kami terima. Kami akan menghubungi via telepon (${phone}) untuk diskusi lebih lanjut mengenai ${product ? '"' + product + '"' : 'kerjasama'}.`);
            this.reset();
        });
        
        // Smooth scroll untuk navigasi
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });
    </script>
</body>
</html>
