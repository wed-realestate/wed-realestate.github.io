<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>عقارات سوريا الجغرافية | المنصة العقارية الحديثة</title>
    <style>
        :root {
            --primary-color: #007a3d; /* الأخضر المستوحى من الهوية السورية */
            --secondary-color: #1e293b;
            --accent-color: #ce1126;  /* الأحمر الحيوي للمسة بصرية حديثة */
            --background: #f8fafc;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            padding: 0;
            background-color: var(--background);
            color: var(--secondary-color);
        }

        /* شريط التنقل */
        header {
            background: white;
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
            padding: 15px 5%;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 24px;
            font-weight: bold;
            color: var(--primary-color);
            display: flex;
            align-items: center;
            gap: 8px;
        }

        nav a {
            text-decoration: none;
            color: var(--secondary-color);
            margin-right: 20px;
            font-weight: 500;
            transition: color 0.3s;
        }

        nav a:hover {
            color: var(--primary-color);
        }

        /* القسم الرئيسي والبحث المخصص للمحافظات */
        .hero {
            background: linear-gradient(rgba(30, 41, 59, 0.65), rgba(30, 41, 59, 0.65)), url('https://images.unsplash.com/photo-1549693578-d683be217e58?auto=format&fit=crop&w=1200&q=80');
            background-size: cover;
            background-position: center;
            height: 480px;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            color: white;
            text-align: center;
            padding: 0 20px;
        }

        .hero h1 { font-size: 38px; margin-bottom: 10px; text-shadow: 0 2px 4px rgba(0,0,0,0.3); }
        .hero p { font-size: 18px; margin-bottom: 25px; }

        .search-container {
            background: white;
            padding: 12px 20px;
            border-radius: 50px;
            display: flex;
            width: 90%;
            max-width: 800px;
            box-shadow: 0 8px 20px rgba(0,0,0,0.2);
            gap: 10px;
        }

        .search-container input, .search-container select {
            border: none;
            outline: none;
            padding: 10px;
            font-size: 16px;
            flex: 1;
            background: transparent;
        }

        .search-container select {
            border-right: 1px solid #e2e8f0;
            padding-right: 15px;
        }

        .search-container button {
            background: var(--primary-color);
            color: white;
            border: none;
            padding: 10px 30px;
            border-radius: 25px;
            cursor: pointer;
            font-size: 16px;
            font-weight: bold;
            transition: background 0.3s;
        }

        .search-container button:hover {
            background: #005c2e;
        }

        /* قسم العقارات الجغرافية */
        .container { padding: 40px 5%; }
        .section-title { font-size: 28px; margin-bottom: 10px; text-align: center; }
        .section-subtitle { text-align: center; color: #64748b; margin-bottom: 40px; }

        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            gap: 30px;
        }

        .card {
            background: white;
            border-radius: 16px;
            overflow: hidden;
            box-shadow: 0 4px 15px rgba(0,0,0,0.05);
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .card:hover { 
            transform: translateY(-5px); 
            box-shadow: 0 8px 25px rgba(0,0,0,0.1);
        }

        .card-img {
            height: 220px;
            background-size: cover;
            background-position: center;
            position: relative;
        }

        .badge-status {
            position: absolute;
            top: 15px;
            right: 15px;
            background: var(--accent-color);
            color: white;
            padding: 6px 14px;
            border-radius: 30px;
            font-size: 13px;
            font-weight: bold;
        }

        .badge-region {
            position: absolute;
            top: 15px;
            left: 15px;
            background: rgba(0, 0, 0, 0.6);
            color: white;
            padding: 6px 14px;
            border-radius: 30px;
            font-size: 13px;
            backdrop-filter: blur(4px);
        }

        .card-content { padding: 25px; }
        .price { color: var(--primary-color); font-size: 22px; font-weight: bold; margin-bottom: 10px; }
        .details { display: flex; gap: 15px; color: #64748b; font-size: 14px; margin-top: 15px; border-top: 1px solid #f1f5f9; padding-top: 15px;}
    </style>
</head>
<body>

    <header>
        <div class="logo">🇸🇾 الخارطة العقارية السورية</div>
        <nav>
            <a href="#">الرئيسية</a>
            <a href="#">عقارات دمشق</a>
            <a href="#">المنطقة الساحلية</a>
            <a href="#">المنطقة الشمالية والوسطى</a>
            <a href="#">أضف عقارك</a>
        </nav>
    </header>

    <div class="hero">
        <h1>بوابتك الذكية للعقارات في سوريا</h1>
        <p>ابحث عن شقق، بيوت مستقلة، ومحاضر تجارية في كافة المحافظات السورية بسهولة</p>
        <div class="search-container">
            <select>
                <option value="">اختر المحافظة</option>
                <option>دمشق وريفها</option>
                <option>حلب</option>
                <option>اللاذقية</option>
                <option>طرطوس</option>
                <option>حمص / حماة</option>
            </select>
            <select>
                <option value="">نوع العقد</option>
                <option>بيع (ملك / فروغ)</option>
                <option>إيجار (سياحي / سنوي)</option>
            </select>
            <input type="text" placeholder="المنطقة أو الحي (مثلاً: مشروع دمر، المزة، الفرقان...)">
            <button>ابحث الآن</button>
        </div>
    </div>

    <div class="container">
        <h2 class="section-title">أحدث العروض الحصرية حسب الجغرافيا السورية</h2>
        <p class="section-subtitle">تصفح العقارات الموثقة جغرافياً وقانونياً</p>
        <div class="grid">
            
            <!-- عقار 1: دمشق -->
            <div class="card">
                <div class="card-img" style="background-image: url('https://images.unsplash.com/photo-1542314831-068cd1dbfeeb?auto=format&fit=crop&w=500&q=80');">
                    <span class="badge-status">للبيع (طابو أخضر)</span>
                    <span class="badge-region">دمشق</span>
                </div>
                <div class="card-content">
                    <div class="price">اتصل لمعرفة السعر</div>
                    <h3>شقة سكنية مخدمة في تنظيم كفرسوسة</h3>
                    <p>إطلالة مميزة، بناء حديث، قريبة من الخدمات الرئيسية والمراكز التجارية.</p>
                    <div class="details">
                        <span>🛏️ 3 غرف نوم</span>
                        <span>🛋️ صالون واسع</span>
                        <span>📐 160 م²</span>
                    </div>
                </div>
            </div>

            <!-- عقار 2: اللاذقية (سياحي) -->
            <div class="card">
                <div class="card-img" style="background-image: url('https://images.unsplash.com/photo-1512917774080-9991f1c4c750?auto=format&fit=crop&w=500&q=80');">
                    <span class="badge-status" style="background: var(--primary-color);">للإيجار السياحي</span>
                    <span class="badge-region">اللاذقية</span>
                </div>
                <div class="card-content">
                    <div class="price">أسعار مناسبة للمواسم</div>
                    <h3>شاليه مودرن نسق أول على البحر</h3>
                    <p>شاطئ الشقيرات، مفروش بالكامل، تكييف متكامل مع طاقة شمسية 24 ساعة.</p>
                    <div class="details">
                        <span>🛏️ 2 غرف نوم</span>
                        <span>🏖️ إطلالة بحرية</span>
                        <span>☀️ طاقة شمسية</span>
                    </div>
                </div>
            </div>

            <!-- عقار 3: حلب -->
            <div class="card">
                <div class="card-img" style="background-image: url('https://images.unsplash.com/photo-1582268611958-ebfd161ef9cf?auto=format&fit=crop&w=500&q=80');">
                    <span class="badge-status">للبيع / الاستثمار</span>
                    <span class="badge-region">حلب</span>
                </div>
                <div class="card-content">
                    <div class="price">بدل استثماري مميز</div>
                    <h3>مكتب تجاري في حي المحافظة</h3>
                    <p>موقع استراتيجي يصلح لعيادة طبية أو مقر شركة، طابق أول فني، كاتب عدل جاهز.</p>
                    <div class="details">
                        <span>🏢 طابق أول</span>
                        <span>🚪 4 غرف مكتبية</span>
                        <span>📐 110 م²</span>
                    </div>
                </div>
            </div>

        </div>
    </div>

</body>
</html>
