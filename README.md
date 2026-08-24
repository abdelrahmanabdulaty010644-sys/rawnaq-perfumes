<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>رونق | للعطور الفاخرة</title>
    <!-- Favicon / اللوجو في شريط المتصفح -->
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
            --text-light: #f8f9fa;
            --text-muted: #a0a0a0;
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
            background: rgba(10, 10, 10, 0.9);
            backdrop-filter: blur(12px);
            padding: 12px 8%;
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
            height: 55px;
            width: auto;
            object-fit: contain;
            border-radius: 6px;
            filter: drop-shadow(0 0 4px rgba(212, 175, 55, 0.4));
        }

        .logo-text {
            font-size: 26px;
            font-weight: 800;
            color: var(--primary);
            letter-spacing: 1.5px;
        }

        nav a {
            color: var(--text-light);
            text-decoration: none;
            margin-right: 25px;
            font-weight: 500;
            transition: color 0.3s;
        }

        nav a:hover {
            color: var(--primary);
        }

        /* Hero Section */
        .hero {
            height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            background: linear-gradient(180deg, rgba(10,10,10,0.55) 0%, rgba(10,10,10,0.95) 100%), 
                        url('https://images.unsplash.com/photo-1592945403244-b3fbafd7f539?q=80&w=1600') center/cover no-repeat;
            padding: 0 20px;
        }

        .hero-logo {
            width: 140px;
            height: auto;
            margin-bottom: 20px;
            border-radius: 12px;
            filter: drop-shadow(0 0 15px rgba(212, 175, 55, 0.5));
        }

        .hero h1 {
            font-size: 52px;
            font-weight: 800;
            color: var(--primary);
            margin-bottom: 12px;
            letter-spacing: 1px;
            text-shadow: 0 4px 15px rgba(0,0,0,0.8);
        }

        .hero p {
            font-size: 22px;
            color: #e0e0e0;
            max-width: 650px;
            margin-bottom: 35px;
            font-weight: 400;
            text-shadow: 0 2px 10px rgba(0,0,0,0.8);
        }

        .btn-main {
            background: linear-gradient(45deg, #d4af37, #f3e5ab);
            color: #000;
            padding: 14px 38px;
            border-radius: 30px;
            font-weight: 700;
            font-size: 16px;
            text-decoration: none;
            box-shadow: 0 4px 20px rgba(212, 175, 55, 0.4);
            transition: all 0.3s ease;
        }

        .btn-main:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 25px rgba(212, 175, 55, 0.6);
        }

        /* Products Section */
        .products {
            padding: 120px 8% 80px;
            text-align: center;
        }

        .section-title {
            font-size: 38px;
            font-weight: 700;
            color: var(--primary);
            margin-bottom: 10px;
        }

        .section-subtitle {
            color: var(--text-muted);
            margin-bottom: 50px;
            font-size: 18px;
        }

        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 35px;
        }

        .card {
            background: var(--card-bg);
            border-radius: 16px;
            padding: 24px;
            border: 1px solid var(--border-color);
            transition: all 0.4s ease;
            position: relative;
            overflow: hidden;
        }

        .card:hover {
            transform: translateY(-8px);
            border-color: var(--primary);
            box-shadow: 0 10px 30px rgba(0,0,0,0.8);
        }

        .card img {
            width: 100%;
            height: 300px;
            object-fit: cover;
            border-radius: 12px;
            margin-bottom: 20px;
        }

        .card h3 {
            font-size: 22px;
            margin-bottom: 8px;
        }

        .card p {
            color: var(--text-muted);
            font-size: 15px;
            margin-bottom: 15px;
        }

        .price {
            color: var(--primary);
            font-weight: 700;
            font-size: 20px;
            margin-bottom: 20px;
        }

        .btn-card {
            display: block;
            background: transparent;
            color: var(--primary);
            border: 1px solid var(--primary);
            padding: 10px;
            border-radius: 25px;
            text-decoration: none;
            font-weight: 600;
            transition: 0.3s;
        }

        .btn-card:hover {
            background: var(--primary);
            color: #000;
        }

        /* Footer & Social Media */
        footer {
            background: #050505;
            padding: 60px 20px 30px;
            text-align: center;
            border-top: 1px solid var(--border-color);
        }

        .footer-logo {
            width: 90px;
            height: auto;
            border-radius: 8px;
            margin-bottom: 15px;
        }

        .footer-title {
            font-size: 22px;
            color: var(--primary);
            margin-bottom: 20px;
            font-weight: 700;
        }

        .social-container {
            display: flex;
            justify-content: center;
            gap: 15px;
            flex-wrap: wrap;
            margin-bottom: 40px;
        }

        .social-btn {
            display: inline-flex;
            align-items: center;
            gap: 10px;
            padding: 12px 24px;
            border-radius: 30px;
            text-decoration: none;
            font-weight: 600;
            color: #fff;
            transition: all 0.3s ease;
            font-size: 15px;
        }

        .facebook { background-color: #1877f2; }
        .whatsapp { background-color: #25d366; }
        .tiktok { background-color: #000000; border: 1px solid #333; }
        .instagram { background: linear-gradient(45deg, #f09433, #e6683c, #dc2743, #cc2366, #bc1888); }

        .social-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(255, 255, 255, 0.15);
            opacity: 0.9;
        }

        .copyright {
            color: var(--text-muted);
            font-size: 14px;
            border-top: 1px solid rgba(255,255,255,0.05);
            padding-top: 20px;
        }
    </style>
</head>
<body>

    <header>
        <a href="#home" class="brand-logo">
            <img src="https://raw.githubusercontent.com/abdelrahmanabdulaty010644-sys/rawnaq-perfumes/main/Screenshot%202026-08-24%20200345.png" alt="لوجو رونق للعطور">
            <span class="logo-text">رونق</span>
        </a>
        <nav>
            <a href="#home">الرئيسية</a>
            <a href="#products">المنتجات</a>
            <a href="#contact">تواصل معنا</a>
        </nav>
    </header>

    <section id="home" class="hero">
        <img src="https://raw.githubusercontent.com/abdelrahmanabdulaty010644-sys/rawnaq-perfumes/main/Screenshot%202026-08-24%20200345.png" alt="رونق للعطور" class="hero-logo">
        <h1>رونق للعطور</h1>
        <p>لمسات خفية تعكس حضورك الأنيق ورونقك الخاص.</p>
        <a href="#products" class="btn-main">اكتشف المجموعة</a>
    </section>

    <section id="products" class="products">
        <h2 class="section-title">تشكيلتنا المميزة</h2>
        <p class="section-subtitle">اختر عطرك المفضل وتميز بحضور لا يُنسى</p>
        
        <div class="grid">
            <div class="card">
                <img src="https://raw.githubusercontent.com/abdelrahmanabdulaty010644-sys/rawnaq-perfumes/main/WhatsApp%20Image%202026-08-24%20at%206.26.35%20PM%20(1).jpeg" alt="عطر رونق 1">
                <h3>عطر رونق الملكي</h3>
                <p>تركيبة عطرية فاخرة تجمع بين الأصالة والجاذبية.</p>
                <div class="price">450 جنيه</div>
                <a href="https://chat.whatsapp.com/Ett4jGXBrtl2retP8XNy4X?s=sh&p=a&ilr=0&amv=0" target="_blank" class="btn-card">
                    <i class="fa-brands fa-whatsapp"></i> اطلب عبر الواتساب
                </a>
            </div>
            
            <div class="card">
                <img src="https://raw.githubusercontent.com/abdelrahmanabdulaty010644-sys/rawnaq-perfumes/main/WhatsApp%20Image%202026-08-24%20at%206.26.35%20PM.jpeg" alt="عطر رونق 2">
                <h3>رونق العود والمسك</h3>
                <p>مزيج ساحر ينبض بالفخامة والانتعاش طوال اليوم.</p>
                <div class="price">380 جنيه</div>
                <a href="https://chat.whatsapp.com/Ett4jGXBrtl2retP8XNy4X?s=sh&p=a&ilr=0&amv=0" target="_blank" class="btn-card">
                    <i class="fa-brands fa-whatsapp"></i> اطلب عبر الواتساب
                </a>
            </div>

            <div class="card">
                <img src="https://raw.githubusercontent.com/abdelrahmanabdulaty010644-sys/rawnaq-perfumes/main/WhatsApp%20Image%202026-08-24%20at%206.26.36%20PM%20(1).jpeg" alt="عطر رونق 3">
                <h3>رونق الفانيلا والزهور</h3>
                <p>نفحات دافئة ورقيقة تأسر الحواس برقتها.</p>
                <div class="price">400 جنيه</div>
                <a href="https://chat.whatsapp.com/Ett4jGXBrtl2retP8XNy4X?s=sh&p=a&ilr=0&amv=0" target="_blank" class="btn-card">
                    <i class="fa-brands fa-whatsapp"></i> اطلب عبر الواتساب
                </a>
            </div>

            <div class="card">
                <img src="https://raw.githubusercontent.com/abdelrahmanabdulaty010644-sys/rawnaq-perfumes/main/WhatsApp%20Image%202026-08-24%20at%206.26.36%20PM%20(2).jpeg" alt="عطر رونق 4">
                <h3>رونق المورينجا والندى</h3>
                <p>لمسة منعشة وعصرية تعكس التميز والأناقة.</p>
                <div class="price">420 جنيه</div>
                <a href="https://chat.whatsapp.com/Ett4jGXBrtl2retP8XNy4X?s=sh&p=a&ilr=0&amv=0" target="_blank" class="btn-card">
                    <i class="fa-brands fa-whatsapp"></i> اطلب عبر الواتساب
                </a>
            </div>

            <div class="card">
                <img src="https://raw.githubusercontent.com/abdelrahmanabdulaty010644-sys/rawnaq-perfumes/main/WhatsApp%20Image%202026-08-24%20at%206.26.36%20PM%20(3).jpeg" alt="عطر رونق 5">
                <h3>رونق بلاك نايت</h3>
                <p>عطر رسمي فخم مخصص للسهرات والمناسبات الخاصة.</p>
                <div class="price">480 جنيه</div>
                <a href="https://chat.whatsapp.com/Ett4jGXBrtl2retP8XNy4X?s=sh&p=a&ilr=0&amv=0" target="_blank" class="btn-card">
                    <i class="fa-brands fa-whatsapp"></i> اطلب عبر الواتساب
                </a>
            </div>

            <div class="card">
                <img src="https://raw.githubusercontent.com/abdelrahmanabdulaty010644-sys/rawnaq-perfumes/main/WhatsApp%20Image%202026-08-24%20at%206.26.36%20PM.jpeg" alt="عطر رونق 6">
                <h3>مجموعة رونق الخاصة</h3>
                <p>إصدار محدود لعشاق التميز والعطور الفاخرة.</p>
                <div class="price">500 جنيه</div>
                <a href="https://chat.whatsapp.com/Ett4jGXBrtl2retP8XNy4X?s=sh&p=a&ilr=0&amv=0" target="_blank" class="btn-card">
                    <i class="fa-brands fa-whatsapp"></i> اطلب عبر الواتساب
                </a>
            </div>
        </div>
    </section>

    <footer id="contact">
        <img src="https://raw.githubusercontent.com/abdelrahmanabdulaty010644-sys/rawnaq-perfumes/main/Screenshot%202026-08-24%20200345.png" alt="لوجو رونق" class="footer-logo">
        <h3 class="footer-title">تابع براند رونق على منصات التواصل</h3>
        
        <div class="social-container">
            <a href="https://www.facebook.com/share/1bGxj2MaW6/" target="_blank" rel="noopener noreferrer" class="social-btn facebook">
                <i class="fa-brands fa-facebook-f"></i> فيسبوك
            </a>
            <a href="https://www.instagram.com/rawnaq_perfume10?igsh=NWxlazBocHJkNmFh" target="_blank" rel="noopener noreferrer" class="social-btn instagram">
                <i class="fa-brands fa-instagram"></i> انستجرام
            </a>
            <a href="https://vt.tiktok.com/ZSXr9sehd/" target="_blank" rel="noopener noreferrer" class="social-btn tiktok">
                <i class="fa-brands fa-tiktok"></i> تيك توك
            </a>
            <a href="https://chat.whatsapp.com/Ett4jGXBrtl2retP8XNy4X?s=sh&p=a&ilr=0&amv=0" target="_blank" rel="noopener noreferrer" class="social-btn whatsapp">
                <i class="fa-brands fa-whatsapp"></i> مجتمع الواتساب
            </a>
        </div>

        <p class="copyright">جميع الحقوق محفوظة &copy; 2026 براند رونق للعطور</p>
    </footer>

</body>
</html>
