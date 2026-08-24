<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>رونق | للعطور الفاخرة والمسكات</title>
    <!-- Favicon -->
    <link rel="icon" type="image/png" href="https://raw.githubusercontent.com/abdelrahmanabdulaty010644-sys/rawnaq-perfumes/main/Screenshot%202026-08-24%20200345.png">
    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Tajawal:wght@300;400;500;700;800&display=swap" rel="stylesheet">
    <!-- FontAwesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <style>
        :root {
            --primary: #d4af37;
            --primary-hover: #f3e5ab;
            --bg-dark: #0a0a0a;
            --card-bg: #141414;
            --text-light: #ffffff;
            --text-muted: #b0b0b0;
            --border-color: rgba(212, 175, 55, 0.25);
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Tajawal', sans-serif;
            scroll-behavior: smooth;
        }

        body {
            background-color: var(--bg-dark);
            color: var(--text-light);
            line-height: 1.7;
            overflow-x: hidden;
        }

        /* Header & Nav */
        header {
            background: rgba(10, 10, 10, 0.95);
            backdrop-filter: blur(12px);
            padding: 12px 6%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            border-bottom: 1px solid var(--border-color);
        }

        .brand-logo {
            display: flex;
            align-items: center;
            gap: 12px;
            text-decoration: none;
        }

        .brand-logo img {
            height: 50px;
            width: auto;
            border-radius: 6px;
        }

        .logo-text {
            font-size: 24px;
            font-weight: 800;
            color: var(--primary);
        }

        nav a {
            color: var(--text-light);
            text-decoration: none;
            margin-right: 20px;
            font-weight: 500;
            transition: color 0.3s;
        }

        nav a:hover {
            color: var(--primary);
        }

        /* Hero Section */
        .hero {
            height: 70vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            background: linear-gradient(180deg, rgba(10,10,10,0.75) 0%, rgba(10,10,10,0.95) 100%), 
                        url('https://raw.githubusercontent.com/abdelrahmanabdulaty010644-sys/rawnaq-perfumes/main/WhatsApp%20Image%202026-08-24%20at%206.26.36%20PM.jpeg') center/cover no-repeat;
            padding: 100px 20px 40px;
        }

        .hero-logo {
            width: 110px;
            height: auto;
            border-radius: 12px;
            margin-bottom: 15px;
            filter: drop-shadow(0 0 10px rgba(212, 175, 55, 0.5));
        }

        .hero h1 {
            font-size: 44px;
            font-weight: 800;
            color: var(--primary);
            margin-bottom: 10px;
        }

        .hero p {
            font-size: 18px;
            color: #e0e0e0;
            max-width: 600px;
            margin-bottom: 25px;
        }

        /* Pricing Section */
        .pricing-section {
            padding: 60px 6%;
            background: #0f0f0f;
            border-bottom: 1px solid var(--border-color);
        }

        .section-title {
            font-size: 32px;
            font-weight: 700;
            color: var(--primary);
            text-align: center;
            margin-bottom: 10px;
        }

        .section-subtitle {
            color: var(--text-muted);
            text-align: center;
            margin-bottom: 35px;
            font-size: 16px;
        }

        .price-tables-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 25px;
        }

        .price-card {
            background: var(--card-bg);
            border: 1px solid var(--border-color);
            border-radius: 12px;
            padding: 20px;
        }

        .price-card h3 {
            color: var(--primary);
            margin-bottom: 15px;
            text-align: center;
            font-size: 20px;
            border-bottom: 1px solid var(--border-color);
            padding-bottom: 8px;
        }

        /* تعديل الجدول ليكون كل النص (الحجم والسعر) باللون الذهبي الواضح */
        .price-table {
            width: 100%;
            border-collapse: collapse;
            text-align: right;
            background-color: #1a1a1a;
            border-radius: 8px;
            overflow: hidden;
        }

        .price-table th {
            background-color: #222222;
            color: var(--primary);
            font-weight: 700;
            padding: 12px;
            border-bottom: 1px solid var(--border-color);
        }

        .price-table td {
            padding: 12px;
            border-bottom: 1px solid rgba(255, 255, 255, 0.08);
            font-size: 15px;
            color: var(--primary) !important; /* لون ذهبي ناصع لكل الخانات */
            font-weight: 600;
        }

        .price-table tr:hover {
            background-color: rgba(212, 175, 55, 0.08);
        }

        /* Products Section & Filters */
        .products-section {
            padding: 60px 6%;
        }

        .filter-container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 10px;
            margin-bottom: 40px;
        }

        .filter-btn {
            background: var(--card-bg);
            border: 1px solid var(--border-color);
            color: var(--text-light);
            padding: 8px 18px;
            border-radius: 20px;
            cursor: pointer;
            font-size: 14px;
            font-weight: 600;
            transition: all 0.3s ease;
        }

        .filter-btn:hover, .filter-btn.active {
            background: var(--primary);
            color: #000;
            border-color: var(--primary);
        }

        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
            gap: 25px;
        }

        .card {
            background: var(--card-bg);
            border-radius: 12px;
            padding: 20px;
            border: 1px solid var(--border-color);
            transition: all 0.3s ease;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
        }

        .card:hover {
            transform: translateY(-5px);
            border-color: var(--primary);
        }

        .card img {
            width: 100%;
            height: 240px;
            object-fit: cover;
            border-radius: 8px;
            margin-bottom: 15px;
        }

        .card-tags {
            display: flex;
            gap: 6px;
            flex-wrap: wrap;
            margin-bottom: 10px;
        }

        .tag {
            font-size: 11px;
            padding: 3px 8px;
            border-radius: 12px;
            background: rgba(212, 175, 55, 0.15);
            color: var(--primary);
            border: 1px solid rgba(212, 175, 55, 0.3);
        }

        .card h3 {
            font-size: 19px;
            margin-bottom: 6px;
        }

        .card-notes {
            font-size: 13px;
            color: var(--text-muted);
            margin-bottom: 12px;
            min-height: 38px;
        }

        .card-price-info {
            font-size: 14px;
            color: var(--primary);
            font-weight: 700;
            margin-bottom: 15px;
            background: rgba(0,0,0,0.3);
            padding: 8px;
            border-radius: 6px;
            text-align: center;
        }

        .btn-card {
            display: block;
            text-align: center;
            background: transparent;
            color: var(--primary);
            border: 1px solid var(--primary);
            padding: 8px;
            border-radius: 20px;
            text-decoration: none;
            font-weight: 600;
            font-size: 14px;
            transition: 0.3s;
        }

        .btn-card:hover {
            background: var(--primary);
            color: #000;
        }

        /* Footer */
        footer {
            background: #050505;
            padding: 40px 20px 20px;
            text-align: center;
            border-top: 1px solid var(--border-color);
        }

        .footer-logo {
            width: 70px;
            height: auto;
            border-radius: 6px;
            margin-bottom: 10px;
        }

        .social-container {
            display: flex;
            justify-content: center;
            gap: 12px;
            flex-wrap: wrap;
            margin: 20px 0;
        }

        .social-btn {
            display: inline-flex;
            align-items: center;
            gap: 8px;
            padding: 8px 18px;
            border-radius: 20px;
            text-decoration: none;
            font-weight: 600;
            color: #fff;
            font-size: 13px;
        }

        .facebook { background-color: #1877f2; }
        .whatsapp { background-color: #25d366; }
        .tiktok { background-color: #000; border: 1px solid #333; }
        .instagram { background: linear-gradient(45deg, #f09433, #e6683c, #dc2743, #cc2366, #bc1888); }

        .copyright {
            color: var(--text-muted);
            font-size: 13px;
            border-top: 1px solid rgba(255,255,255,0.05);
            padding-top: 15px;
        }
    </style>
</head>
<body>

    <header>
        <a href="#home" class="brand-logo">
            <img src="https://raw.githubusercontent.com/abdelrahmanabdulaty010644-sys/rawnaq-perfumes/main/Screenshot%202026-08-24%20200345.png" alt="لوجو رونق">
            <span class="logo-text">رونق</span>
        </a>
        <nav>
            <a href="#home">الرئيسية</a>
            <a href="#prices">قائمة الأسعار</a>
            <a href="#products">الكتالوج الكامل</a>
            <a href="#contact">تواصل معنا</a>
        </nav>
    </header>

    <section id="home" class="hero">
        <img src="https://raw.githubusercontent.com/abdelrahmanabdulaty010644-sys/rawnaq-perfumes/main/Screenshot%202026-08-24%20200345.png" alt="رونق للعطور" class="hero-logo">
        <h1>رونق للعطور والمسكات</h1>
        <p>تشكيلة فاخرة مقسمة حسب التصنيف العطري والموسم ونوع العطر لتختار ما يناسب ذوقك ورونقك الخاص.</p>
    </section>

    <!-- Pricing Section -->
    <section id="prices" class="pricing-section">
        <h2 class="section-title">قائمة الأسعار الرسمية</h2>
        <p class="section-subtitle">أسعار العطور والمسكات بحسب حجم الزجاجة والفئة</p>
        
        <div class="price-tables-grid">
            <div class="price-card">
                <h3><i class="fa-solid fa-spray-can"></i> العطور العادية</h3>
                <table class="price-table">
                    <thead>
                        <tr><th>الفئة / الحجم</th><th>السعر</th></tr>
                    </thead>
                    <tbody>
                        <tr><td>تستر 5 مل</td><td>25 ج.م</td></tr>
                        <tr><td>تستر 10 مل</td><td>40 ج.م</td></tr>
                        <tr><td>زجاجة تعبان 30 مل</td><td>80 ج.م</td></tr>
                        <tr><td>زجاجة تعبان 50 مل</td><td>150 ج.م</td></tr>
                        <tr><td>زجاجة بريميوم 30 مل</td><td>150 ج.م</td></tr>
                        <tr><td>زجاجة بريميوم 50 مل</td><td>250 ج.م</td></tr>
                        <tr><td>زجاجة بريميوم 100 مل</td><td>350 ج.م</td></tr>
                    </tbody>
                </table>
            </div>

            <div class="price-card">
                <h3><i class="fa-solid fa-gem"></i> الاصدارات الخاصة (عود مضاوي / خمرة / اربابورا)</h3>
                <table class="price-table">
                    <thead>
                        <tr><th>الفئة / الحجم</th><th>السعر</th></tr>
                    </thead>
                    <tbody>
                        <tr><td>تستر 5 مل</td><td>30 ج.م</td></tr>
                        <tr><td>تستر 10 مل</td><td>50 ج.م</td></tr>
                        <tr><td>زجاجة تعبان 30 مل</td><td>200 ج.م</td></tr>
                        <tr><td>زجاجة تعبان 50 مل</td><td>300 ج.م</td></tr>
                        <tr><td>زجاجة بريميوم 30 مل</td><td>250 ج.م</td></tr>
                        <tr><td>زجاجة بريميوم 50 مل</td><td>350 ج.م</td></tr>
                        <tr><td>زجاجة بريميوم 100 مل</td><td>500 ج.م</td></tr>
                    </tbody>
                </table>
            </div>

            <div class="price-card">
                <h3><i class="fa-solid fa-bottle-droplet"></i> أسعار رول المسك</h3>
                <table class="price-table">
                    <thead>
                        <tr><th>الحجم</th><th>سعر القطعة</th><th>باكدج (5 قطع)</th></tr>
                    </thead>
                    <tbody>
                        <tr><td>1.5 مل</td><td>10 ج.م</td><td>50 ج.م</td></tr>
                        <tr><td>2.5 مل</td><td>15 ج.م</td><td>75 ج.م</td></tr>
                        <tr><td>5 مل</td><td>30 ج.م</td><td>150 ج.م</td></tr>
                        <tr><td>7 مل</td><td>40 ج.م</td><td>200 ج.م</td></tr>
                    </tbody>
                </table>
            </div>
        </div>
    </section>

    <!-- Products Catalog Section -->
    <section id="products" class="products-section">
        <h2 class="section-title">كتالوج المنتجات التصنيفي</h2>
        <p class="section-subtitle">اختر التصنيف أو النوع لعرض العطور والمسكات الخاصة به</p>

        <!-- Filters -->
        <div class="filter-container">
            <button class="filter-btn active" onclick="filterProducts('all')">الكل</button>
            <button class="filter-btn" onclick="filterProducts('حريمي')">عطور حريمي</button>
            <button class="filter-btn" onclick="filterProducts('رجالي')">عطور رجالي</button>
            <button class="filter-btn" onclick="filterProducts('يونيسكس')">يونيسكس</button>
            <button class="filter-btn" onclick="filterProducts('مسك')">المسكات</button>
            <button class="filter-btn" onclick="filterProducts('شتوي')">شتوي / دافئ</button>
            <button class="filter-btn" onclick="filterProducts('صيفي')">صيفي / فريش</button>
            <button class="filter-btn" onclick="filterProducts('شوغري')">شوغري / غورماند</button>
        </div>

        <div class="grid" id="products-grid">
            <!-- JS dynamic content injection -->
        </div>
    </section>

    <footer id="contact">
        <img src="https://raw.githubusercontent.com/abdelrahmanabdulaty010644-sys/rawnaq-perfumes/main/Screenshot%202026-08-24%20200345.png" alt="لوجو رونق" class="footer-logo">
        <h3>تابع رونق على منصات التواصل</h3>
        
        <div class="social-container">
            <a href="https://www.facebook.com/share/1bGxj2MaW6/" target="_blank" class="social-btn facebook"><i class="fa-brands fa-facebook-f"></i> فيسبوك</a>
            <a href="https://www.instagram.com/rawnaq_perfume10?igsh=NWxlazBocHJkNmFh" target="_blank" class="social-btn instagram"><i class="fa-brands fa-instagram"></i> انستجرام</a>
            <a href="https://vt.tiktok.com/ZSXr9sehd/" target="_blank" class="social-btn tiktok"><i class="fa-brands fa-tiktok"></i> تيك توك</a>
            <a href="https://chat.whatsapp.com/Ett4jGXBrtl2retP8XNy4X?s=sh&p=a&ilr=0&amv=0" target="_blank" class="social-btn whatsapp"><i class="fa-brands fa-whatsapp"></i> مجتمع الواتساب</a>
        </div>

        <p class="copyright">جميع الحقوق محفوظة &copy; 2026 رونق للعطور</p>
    </footer>

    <script>
        const productsData = [
            { name: "يارا كاندي", type: "حريمي", season: "صيفي/ربيعي", category: "شوغري • فاكهي • فلاوري", notes: "كشمش أسود، يوسفي أخضر، حلوى فراولة، جاردينيا، فانيليا، مسك", price: "يبدأ من 25 ج.م (تستر) / 80 ج.م (زجاجة)", image: "https://raw.githubusercontent.com/abdelrahmanabdulaty010644-sys/rawnaq-perfumes/main/WhatsApp%20Image%202026-08-24%20at%206.26.35%20PM%20(1).jpeg", group: ["حريمي", "صيفي", "شوغري"] },
            { name: "اسكندل نايت", type: "حريمي", season: "شتوي/ليلي", category: "حلو • عنبري • فلاوري", notes: "عسل، أزهار بيضاء، عنبر فاخر", price: "يبدأ من 25 ج.م (تستر) / 80 ج.م (زجاجة)", image: "https://raw.githubusercontent.com/abdelrahmanabdulaty010644-sys/rawnaq-perfumes/main/WhatsApp%20Image%202026-08-24%20at%206.26.35%20PM.jpeg", group: ["حريمي", "شتوي", "شوغري"] },
            { name: "جوتشي روشي (Gucci Rush)", type: "حريمي", season: "ربيعي/خريفي", category: "فلاوري • فاكهي • حلو", notes: "خوخ، فريزيا، جاردينيا، ياسمين، ورد، باتشولي، فانيليا", price: "يبدأ من 25 ج.م (تستر) / 80 ج.م (زجاجة)", image: "https://raw.githubusercontent.com/abdelrahmanabdulaty010644-sys/rawnaq-perfumes/main/WhatsApp%20Image%202026-08-24%20at%206.26.36%20PM%20(1).jpeg", group: ["حريمي", "صيفي"] },
            { name: "The Only One (D&G)", type: "حريمي", season: "خريفي/شتوي", category: "غورماند • فلاوري • قهوة", notes: "بنفسجي، قهوة، زهر البرتقال، كمثرى، ورد، فانيليا", price: "يبدأ من 25 ج.م (تستر) / 80 ج.م (زجاجة)", image: "https://raw.githubusercontent.com/abdelrahmanabdulaty010644-sys/rawnaq-perfumes/main/WhatsApp%20Image%202026-08-24%20at%206.26.36%20PM%20(2).jpeg", group: ["حريمي", "شتوي", "شوغري"] },
            { name: "سلفر سنت", type: "رجالي", season: "صيفي/ربيعي", category: "فريش • حمضي • وودي", notes: "ليمون، برتقال، لافندر، إكليل الجبل، كزبرة، خشب الساج", price: "يبدأ من 25 ج.م (تستر) / 80 ج.م (زجاجة)", image: "https://raw.githubusercontent.com/abdelrahmanabdulaty010644-sys/rawnaq-perfumes/main/WhatsApp%20Image%202026-08-24%20at%206.26.36%20PM%20(3).jpeg", group: ["رجالي", "صيفي"] },
            { name: "عود مضاوي", type: "يونيسكس", season: "شتوي", category: "عودي • خشبي • شرقي", notes: "عود، أخشاب، عنبر، توابل، مسك فاخر", price: "خاص: 30 ج.م (تستر) / 200 ج.م (زجاجة)", image: "https://raw.githubusercontent.com/abdelrahmanabdulaty010644-sys/rawnaq-perfumes/main/WhatsApp%20Image%202026-08-24%20at%206.26.36%20PM.jpeg", group: ["يونيسكس", "شتوي"] },
            { name: "بكارات روج", type: "يونيسكس", season: "كل المواسم", category: "عنبرى • خشبي • مسكي", notes: "زعفران، ياسمين، عنبر وود، أرز، أمبروكسان", price: "يبدأ من 25 ج.م (تستر) / 80 ج.م (زجاجة)", image: "https://raw.githubusercontent.com/abdelrahmanabdulaty010644-sys/rawnaq-perfumes/main/WhatsApp%20Image%202026-08-24%20at%206.26.35%20PM%20(1).jpeg", group: ["يونيسكس", "شتوي"] },
            { name: "استرونجر وز يو", type: "رجالي", season: "خريفي/شتوي", category: "عنبرى • حلو • وودي", notes: "كستناء، فلفل وردي، سالفيا، فانيليا، أمبروود", price: "يبدأ من 25 ج.م (تستر) / 80 ج.م (زجاجة)", image: "https://raw.githubusercontent.com/abdelrahmanabdulaty010644-sys/rawnaq-perfumes/main/WhatsApp%20Image%202026-08-24%20at%206.26.35%20PM.jpeg", group: ["رجالي", "شتوي", "شوغري"] },
            { name: "سوفاج", type: "رجالي", season: "صيفي/ربيعي", category: "فريش • سبايسي • وودي", notes: "برغموت، فلفل، أمبروكسان، لافندر، أخشاب", price: "يبدأ من 25 ج.م (تستر) / 80 ج.م (زجاجة)", image: "https://raw.githubusercontent.com/abdelrahmanabdulaty010644-sys/rawnaq-perfumes/main/WhatsApp%20Image%202026-08-24%20at%206.26.36%20PM%20(1).jpeg", group: ["رجالي", "صيفي"] },
            { name: "جود جيرل", type: "حريمي", season: "خريفي/شتوي", category: "غورماند • فلاوري • حلو", notes: "لوز، قهوة، ياسمين سامباك، تونكا، كاكاو، فانيليا", price: "يبدأ من 25 ج.م (تستر) / 80 ج.م (زجاجة)", image: "https://raw.githubusercontent.com/abdelrahmanabdulaty010644-sys/rawnaq-perfumes/main/WhatsApp%20Image%202026-08-24%20at%206.26.36%20PM%20(2).jpeg", group: ["حريمي", "شتوي", "شوغري"] },
            { name: "خمره", type: "يونيسكس", season: "شتوي", category: "غورماند • سبايسي • حلو", notes: "قرفة، جوزة الطيب، فانيليا، كراميل، عنبر", price: "خاص: 30 ج.م (تستر) / 200 ج.م (زجاجة)", image: "https://raw.githubusercontent.com/abdelrahmanabdulaty010644-sys/rawnaq-perfumes/main/WhatsApp%20Image%202026-08-24%20at%206.26.36%20PM%20(3).jpeg", group: ["يونيسكس", "شتوي", "شوغري"] },
            { name: "اربابورا", type: "يونيسكس", season: "صيفي/ربيعي", category: "فاكهي • حمضي • مسكي", notes: "برتقال سيسيلي، ليمون، فواكه استوائية، مسك أبيض، فانيليا", price: "خاص: 30 ج.م (تستر) / 200 ج.م (زجاجة)", image: "https://raw.githubusercontent.com/abdelrahmanabdulaty010644-sys/rawnaq-perfumes/main/WhatsApp%20Image%202026-08-24%20at%206.26.36%20PM.jpeg", group: ["يونيسكس", "صيفي"] },
            { name: "مسك فراولة", type: "يونيسكس", season: "صيفي/ربيعي", category: "فاكهي • شوغري • مسكي", notes: "مسك أبيض فاخر ناعم مع نفحات الفراولة الحلوة", price: "رول مسك من 10 ج.م / زجاجات من 80 ج.م", image: "https://raw.githubusercontent.com/abdelrahmanabdulaty010644-sys/rawnaq-perfumes/main/WhatsApp%20Image%202026-08-24%20at%206.26.35%20PM%20(1).jpeg", group: ["مسك", "صيفي", "شوغري"] },
            { name: "مسك رمان", type: "يونيسكس", season: "صيفي/ربيعي", category: "فاكهي • حلو • مسكي", notes: "مسك النظافة الفاخر ممزوج بالرمان المنعش", price: "رول مسك من 10 ج.م / زجاجات من 80 ج.م", image: "https://raw.githubusercontent.com/abdelrahmanabdulaty010644-sys/rawnaq-perfumes/main/WhatsApp%20Image%202026-08-24%20at%206.26.35%20PM.jpeg", group: ["مسك", "صيفي"] },
            { name: "مسك كعبه", type: "يونيسكس", season: "كل المواسم", category: "مسكي • بودري • نظيف", notes: "مسك أسود فاخر بنفحات شرقية روحانية مميزة", price: "رول مسك من 10 ج.م / زجاجات من 80 ج.م", image: "https://raw.githubusercontent.com/abdelrahmanabdulaty010644-sys/rawnaq-perfumes/main/WhatsApp%20Image%202026-08-24%20at%206.26.36%20PM%20(1).jpeg", group: ["مسك", "شتوي"] }
        ];

        function renderProducts(items) {
            const grid = document.getElementById('products-grid');
            grid.innerHTML = items.map(item => `
                <div class="card">
                    <div>
                        <img src="${item.image}" alt="${item.name}">
                        <div class="card-tags">
                            <span class="tag">${item.type}</span>
                            <span class="tag">${item.season}</span>
                        </div>
                        <h3>${item.name}</h3>
                        <p style="color: var(--primary); font-size: 12px; margin-bottom: 6px;">${item.category}</p>
                        <p class="card-notes">${item.notes}</p>
                    </div>
                    <div>
                        <div class="card-price-info">${item.price}</div>
                        <a href="https://chat.whatsapp.com/Ett4jGXBrtl2retP8XNy4X?s=sh&p=a&ilr=0&amv=0" target="_blank" class="btn-card">
                            <i class="fa-brands fa-whatsapp"></i> اطلب الآن
                        </a>
                    </div>
                </div>
            `).join('');
        }

        function filterProducts(filter) {
            document.querySelectorAll('.filter-btn').forEach(btn => btn.classList.remove('active'));
            event.target.classList.add('active');

            if (filter === 'all') {
                renderProducts(productsData);
            } else {
                const filtered = productsData.filter(item => item.group.includes(filter) || item.type.includes(filter));
                renderProducts(filtered);
            }
        }

        // Initial Load
        renderProducts(productsData);
    </script>
</body>
</html>
