---
layout: page
title: کتابخانه کیهانی - فصل سوم
subtitle: سرخ‌گرایی کیهانی | اثر داپلر | طیف‌بینی
show_sidebar: false
# hero_image: ../../img/cmb.jpg
---

<style>
@import url('https://cdn.jsdelivr.net/gh/rastikerdar/vazir-font@v30.1.0/dist/font-face.css');

.cosmic-library {
    font-family: 'Vazir', 'Segoe UI', Tahoma, sans-serif;
    max-width: 1200px;
    margin: 0 auto;
    padding: 20px;
    direction: rtl;
    color: #1a3c6e;
}

/* هدر فصل */
.chapter-header {
    background: linear-gradient(135deg, #4a0e0e 0%, #8b1a1a 100%);
    color: white;
    padding: 40px;
    border-radius: 30px;
    margin-bottom: 40px;
    position: relative;
    overflow: hidden;
    box-shadow: 0 15px 30px rgba(139, 26, 26, 0.3);
}

.chapter-header::before {
    content: "🔴";
    position: absolute;
    left: 20px;
    top: 20px;
    font-size: 80px;
    opacity: 0.2;
}

.chapter-title {
    font-size: 2.5rem;
    font-weight: bold;
    margin-bottom: 10px;
}

.chapter-subtitle {
    font-size: 1.2rem;
    opacity: 0.9;
}

/* بخش‌های محتوا */
.content-section {
    background: white;
    border-radius: 20px;
    padding: 30px;
    margin-bottom: 30px;
    box-shadow: 0 5px 20px rgba(0,0,0,0.05);
    border: 1px solid #e1ecf4;
}

.section-title {
    color: #1a3c6e;
    font-size: 1.8rem;
    margin-bottom: 25px;
    padding-right: 15px;
    border-right: 5px solid #8b1a1a;
    display: flex;
    align-items: center;
    gap: 10px;
}

.section-title span {
    background: #8b1a1a;
    color: white;
    padding: 5px 15px;
    border-radius: 30px;
    font-size: 1rem;
}

/* لیست منابع */
.resources-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(350px, 1fr));
    gap: 15px;
}

.resource-item {
    display: flex;
    align-items: center;
    padding: 12px 18px;
    background: #f8fafc;
    border-radius: 12px;
    transition: all 0.2s;
    border: 1px solid transparent;
}

.resource-item:hover {
    background: #fff0f0;
    border-color: #8b1a1a;
    transform: translateX(-5px);
}

.resource-icon {
    font-size: 1.5rem;
    margin-left: 12px;
    color: #8b1a1a;
}

.resource-link {
    color: #1a3c6e;
    text-decoration: none;
    font-size: 0.95rem;
    line-height: 1.6;
    flex: 1;
}

.resource-link:hover {
    color: #8b1a1a;
}

.resource-tag {
    background: #ffe6e6;
    color: #8b1a1a;
    padding: 3px 10px;
    border-radius: 20px;
    font-size: 0.75rem;
    margin-right: 10px;
    white-space: nowrap;
}

/* بخش ویدیوی ویژه */
.featured-video {
    background: linear-gradient(135deg, #fff5f5 0%, #ffe6e6 100%);
    border-radius: 20px;
    padding: 30px;
    margin: 30px 0;
    border: 2px solid #8b1a1a;
    position: relative;
    overflow: hidden;
}

.featured-video::before {
    content: "🚑";
    position: absolute;
    left: 20px;
    bottom: 20px;
    font-size: 60px;
    opacity: 0.1;
}

.featured-title {
    color: #8b1a1a;
    font-size: 1.5rem;
    margin-bottom: 15px;
    display: flex;
    align-items: center;
    gap: 10px;
}

.featured-description {
    background: white;
    padding: 20px;
    border-radius: 16px;
    margin: 15px 0;
    border-right: 4px solid #8b1a1a;
}

.featured-quote {
    font-style: italic;
    color: #4a6fa5;
    margin: 15px 0;
    padding-right: 20px;
    border-right: 3px solid #8b1a1a;
}

.featured-link {
    display: inline-flex;
    align-items: center;
    gap: 10px;
    background: #8b1a1a;
    color: white;
    padding: 12px 25px;
    border-radius: 30px;
    text-decoration: none;
    font-weight: bold;
    margin-top: 15px;
    transition: all 0.2s;
}

.featured-link:hover {
    background: #5e1212;
    transform: scale(1.05);
}

/* بخش تصاویر ویژه */
.image-showcase {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
    margin: 20px 0;
    justify-content: center;
}

.image-card {
    flex: 1;
    min-width: 300px;
    background: white;
    border-radius: 16px;
    padding: 20px;
    box-shadow: 0 5px 15px rgba(0,0,0,0.05);
    border: 1px solid #e1ecf4;
    text-align: center;
}

.image-card img {
    max-width: 100%;
    border-radius: 12px;
    margin-bottom: 15px;
    border: 1px solid #e1ecf4;
}

.image-card .image-caption {
    color: #4a6fa5;
    font-size: 0.9rem;
    margin-top: 10px;
}

.image-card .image-credit {
    color: #6c757d;
    font-size: 0.8rem;
    margin-top: 5px;
}

.image-link {
    display: inline-block;
    margin-top: 10px;
    color: #2c5aa0;
    text-decoration: none;
    font-size: 0.9rem;
}

.image-link:hover {
    text-decoration: underline;
}

/* کارت تعاملی ویژه */
.interactive-card {
    background: linear-gradient(135deg, #ff9999 0%, #ff6b6b 100%);
    color: white;
    padding: 25px;
    border-radius: 20px;
    text-align: center;
}

.interactive-card a {
    color: white;
    font-weight: bold;
    text-decoration: none;
    font-size: 1.3rem;
}

.interactive-card:hover {
    transform: scale(1.02);
}

/* اینفوگرافیک */
.infographic-card {
    background: linear-gradient(135deg, #2c3e50 0%, #34495e 100%);
    color: white;
    padding: 25px;
    border-radius: 20px;
    text-align: center;
}

.infographic-card a {
    color: white;
    font-weight: bold;
    text-decoration: none;
    font-size: 1.3rem;
}

/* کارت آشپزخانه کیهان */
.kitchen-card {
    background: linear-gradient(135deg, #f7971e 0%, #ffd200 100%);
    color: #1a3c6e;
    padding: 25px;
    border-radius: 20px;
    text-align: center;
    margin: 20px 0;
}

.kitchen-card a {
    color: #1a3c6e;
    font-weight: bold;
    text-decoration: none;
    font-size: 1.3rem;
}

.kitchen-card:hover {
    transform: scale(1.02);
}

.kitchen-link {
    display: inline-flex;
    align-items: center;
    gap: 10px;
    background: white;
    color: #1a3c6e;
    padding: 12px 25px;
    border-radius: 30px;
    text-decoration: none;
    font-weight: bold;
    margin: 10px;
    transition: all 0.2s;
    border: 2px solid transparent;
}

.kitchen-link:hover {
    background: #1a3c6e;
    color: white;
    border-color: white;
}

/* بخش‌های ویژه */
.special-section {
    background: linear-gradient(135deg, #fff5f5 0%, #ffe6e6 100%);
    border-radius: 20px;
    padding: 30px;
    margin: 40px 0;
    border: 1px dashed #8b1a1a;
}

.topic-categories {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
    margin-top: 20px;
}

.category-card {
    background: white;
    padding: 20px;
    border-radius: 16px;
    flex: 1;
    min-width: 200px;
    box-shadow: 0 3px 10px rgba(0,0,0,0.02);
    border: 1px solid #ffcdcd;
}

.category-title {
    color: #8b1a1a;
    font-size: 1.2rem;
    font-weight: bold;
    margin-bottom: 10px;
    display: flex;
    align-items: center;
    gap: 8px;
}

.category-items {
    color: #1a3c6e;
    font-size: 0.9rem;
    line-height: 1.8;
}

/* دکمه بازگشت */
.back-button {
    display: inline-block;
    margin-top: 30px;
    padding: 12px 30px;
    background: #8b1a1a;
    color: white;
    text-decoration: none;
    border-radius: 30px;
    transition: all 0.2s;
    border: 2px solid transparent;
}

.back-button:hover {
    background: white;
    color: #8b1a1a;
    border-color: #8b1a1a;
}

/* شمارنده منابع */
.stats-bar {
    display: flex;
    gap: 15px;
    margin-bottom: 30px;
    flex-wrap: wrap;
}

.stat-item {
    background: #ffe6e6;
    padding: 8px 20px;
    border-radius: 30px;
    color: #8b1a1a;
    font-size: 0.9rem;
    display: flex;
    align-items: center;
    gap: 5px;
}

/* ریسپانسیو */
@media (max-width: 768px) {
    .resources-grid {
        grid-template-columns: 1fr;
    }
    
    .chapter-title {
        font-size: 1.8rem;
    }
    
    .topic-categories {
        flex-direction: column;
    }
}
</style>

<div class="cosmic-library" dir="rtl">

<!-- هدر فصل -->
<div class="chapter-header">
    <div class="chapter-title">🔴 فصل سوم: سرخ‌گرایی کیهانی</div>
    <div class="chapter-subtitle">اثر داپلر | انتقال به سرخ | طیف‌بینی | ردشیفت</div>
    <div style="display: flex; gap: 15px; margin-top: 20px; flex-wrap: wrap;">
        <span style="background: rgba(255,255,255,0.2); padding: 5px 15px; border-radius: 30px;">📺 ۱۱ ویدیو</span>
        <span style="background: rgba(255,255,255,0.2); padding: 5px 15px; border-radius: 30px;">🎮 ۳ تعاملی</span>
        <span style="background: rgba(255,255,255,0.2); padding: 5px 15px; border-radius: 30px;">🌐 ۲ وبسایت</span>
        <span style="background: rgba(255,255,255,0.2); padding: 5px 15px; border-radius: 30px;">🖼️ ۱ اینفوگرافیک</span>
    </div>
</div>

<!-- آمار سریع -->
<div class="stats-bar">
    <span class="stat-item">📊 مجموع منابع: ۱۹ منبع</span>
    <span class="stat-item">⏱ مناسب برای: ۵ ساعت آموزش</span>
    <span class="stat-item">🎯 سطح: مبتدی تا متوسط</span>
    <span class="stat-item">🔴 طول موج: افزایش = دور شدن</span>
</div>

<!-- ویدیوی ویژه: اثر داپلر و آژیر آمبولانس -->
<div class="featured-video">
    <div class="featured-title">
        <span>🚑</span> ویدیوی ویژه کلاس درس: اثر داپلر
    </div>
    
    <div style="display: flex; align-items: center; gap: 20px; flex-wrap: wrap;">
        <div style="flex: 1; min-width: 250px;">
            <img src="../../img/doppler-ambulance.jpg" alt="اثر داپلر و آژیر آمبولانس" style="width: 100%; max-width: 300px; border-radius: 16px; box-shadow: 0 8px 20px rgba(0,0,0,0.1);" onerror="this.style.display='none'">
        </div>
        <div style="flex: 2;">
            <div class="featured-description">
                <strong>🎓 گفتگوی کلاسی:</strong>
                <p style="margin-top: 10px;">
                    <span style="background: #8b1a1a; color: white; padding: 3px 10px; border-radius: 20px; font-size: 0.8rem;">دبیر</span>
                    <br>
                    "صبح بخیر دانش‌آموزان! امروز یک سورپرایز کوچک برای شما دارم. می‌خواهم چشمانتان را ببندید و با دقت گوش دهید."
                </p>
                <p style="margin-top: 10px;">
                    <span style="background: #ffc107; color: #1a3c6e; padding: 3px 10px; border-radius: 20px; font-size: 0.8rem;">النا</span>
                    <br>
                    "صدای آژیر آمبولانس بود، اما زیر و بمی صدا وقتی از کنارمان رد شد تغییر کرد."
                </p>
                <p style="margin-top: 10px;">
                    <span style="background: #ffc107; color: #1a3c6e; padding: 3px 10px; border-radius: 20px; font-size: 0.8rem;">والریا</span>
                    <br>
                    "بله، اول صدای زیری داشت و وقتی دور شد، بم‌تر شد."
                </p>
            </div>
            
            <div class="featured-quote">
                <p>📺 این ویدیو اثر داپلر را با صدای آژیر آمبولانس توضیح می‌دهد</p>
            </div>
            
            <a href="https://www.youtube.com/watch?v=rqehO9yfwTA" class="featured-link" target="_blank">
                🎬 تماشای ویدیوی اثر داپلر (آژیر آمبولانس)
                <span style="font-size: 1.2rem;">←</span>
            </a>
        </div>
    </div>
</div>

<!-- 📺 ویدیوها -->
<div class="content-section">
    <div class="section-title">
        📺 ویدیوهای آموزشی <span>۱۱ منبع</span>
    </div>
    <div class="resources-grid">
        <!-- ردیف ۱ - اثر داپلر -->
        <div class="resource-item">
            <span class="resource-icon">🚑</span>
            <a href="https://www.youtube.com/watch?v=ffg4TOpXZyg" class="resource-link" target="_blank">
                <strong>اثر داپلر چگونه کار می‌کند؟</strong>
                <span class="resource-tag">داپلر</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">📡</span>
            <a href="https://www.youtube.com/watch?v=gytA8PuGQo4" class="resource-link" target="_blank">
                <strong>اثر داپلر چیست؟</strong>
                <span class="resource-tag">داپلر</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">🚓</span>
            <a href="https://www.youtube.com/watch?v=ikgRZt1BSyk" class="resource-link" target="_blank">
                <strong>آژیر آمبولانس و تفنگ رادار پلیس</strong>
                <span class="resource-tag">داپلر</span>
            </a>
        </div>
        
        <!-- ردیف ۲ - انتقال به سرخ -->
        <div class="resource-item">
            <span class="resource-icon">🔴</span>
            <a href="https://www.youtube.com/watch?v=-mQ41yA6LaA" class="resource-link" target="_blank">
                <strong>انتقال به سرخ (ردشیفت) چیست؟</strong>
                <span class="resource-tag">ردشیفت</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">🌠</span>
            <a href="https://www.youtube.com/watch?v=_xDETeEA1yE" class="resource-link" target="_blank">
                <strong>انتقال به سرخ - اخترفیزیک</strong>
                <span class="resource-tag">ردشیفت</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">💥</span>
            <a href="https://www.youtube.com/watch?v=bWEtm-7cYzM" class="resource-link" target="_blank">
                <strong>اثر داپلر، انتقال به سرخ و نظریه بیگ‌بنگ</strong>
                <span class="resource-tag">ردشیفت</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">📘</span>
            <a href="https://www.youtube.com/watch?v=mx2M_ZKXM_c" class="resource-link" target="_blank">
                <strong>فیزیک GCSE: انتقال به سرخ چیست؟</strong>
                <span class="resource-tag">ردشیفت</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">📏</span>
            <a href="https://www.youtube.com/watch?v=jjy-eqWM38g" class="resource-link" target="_blank">
                <strong>انتقال به سرخ - مقیاس جهان آکادمی خان</strong>
                <span class="resource-tag">آکادمی خان</span>
            </a>
        </div>
        
        <!-- ردیف ۳ - طیف‌بینی -->
        <div class="resource-item">
            <span class="resource-icon">🌈</span>
            <a href="https://www.youtube.com/watch?v=LYseY0y2tgg" class="resource-link" target="_blank">
                <strong>نور: دوره فشرده نجوم</strong>
                <span class="resource-tag">طیف‌بینی</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">🔬</span>
            <a href="https://www.youtube.com/watch?v=_1mpHBAXh1c" class="resource-link" target="_blank">
                <strong>مقدمه‌ای بر طیف‌بینی - آکادمی خان</strong>
                <span class="resource-tag">طیف‌بینی</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">🔴</span>
            <a href="https://www.youtube.com/watch?v=Y3cTy4HXNmM&t=146s" class="resource-link" target="_blank">
                <strong>انتقال به سرخ: حرکت و رنگ</strong>
                <span class="resource-tag">ردشیفت</span>
            </a>
        </div>
    </div>
</div>

<!-- 🎮 ابزارهای تعاملی -->
<div class="content-section">
    <div class="section-title">
        🎮 ابزارهای تعاملی <span>۳ منبع</span>
    </div>
    <div class="resources-grid">
        <div class="resource-item">
            <span class="resource-icon">⭐</span>
            <a href="https://viewspace.org/interactives/unveiling_invisible_universe/analyzing_light/spectrum_of_the_star_altair" class="resource-link" target="_blank">
                <strong>تحلیل نور: طیف ستاره آلتایر</strong>
                <span class="resource-tag">تعاملی</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">🔄</span>
            <a href="https://foothill.edu/astronomy/astrosims/cosmological-redshift/index.html" class="resource-link" target="_blank">
                <strong>شبیه‌ساز انتقال به سرخ کیهانی</strong>
                <span class="resource-tag">شبیه‌ساز</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">🎨</span>
            <a href="https://readymag.com/u47032242/741098/" class="resource-link" target="_blank">
                <strong>ردیمگ: انتقال به سرخ</strong>
                <span class="resource-tag">تصویری</span>
            </a>
        </div>
    </div>
</div>

<!-- 🌐 وبسایت‌ها -->
<div class="content-section">
    <div class="section-title">
        🌐 وبسایت‌های مرجع <span>۲ منبع</span>
    </div>
    <div class="resources-grid">
        <div class="resource-item">
            <span class="resource-icon">🔭</span>
            <a href="https://hubblesite.org/contents/articles/spectroscopy-reading-the-rainbow" class="resource-link" target="_blank">
                <strong>طیف‌بینی: خواندن رنگین‌کمان</strong>
                <span class="resource-tag">هابل</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">📖</span>
            <a href="https://lco.global/spacebook/light/redshift/" class="resource-link" target="_blank">
                <strong>کتاب فضایی: انتقال به سرخ</strong>
                <span class="resource-tag">LCO</span>
            </a>
        </div>
    </div>
</div>

<!-- 🎬 مستندها -->
<div class="content-section">
    <div class="section-title">
        🎬 مستندهای علمی <span>۳ منبع</span>
    </div>
    <div class="resources-grid">
        <div class="resource-item">
            <span class="resource-icon">🌌</span>
            <a href="https://www.youtube.com/watch?v=68tpCpDOsyA" class="resource-link" target="_blank">
                <strong>سفر به لبه جهان</strong>
                <span class="resource-tag">مستند</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">✨</span>
            <a href="https://topdocumentaryfilms.com/everything-and-nothing/" class="resource-link" target="_blank">
                <strong>همه چیز و هیچ چیز</strong>
                <span class="resource-tag">مستند</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">⚛️</span>
            <a href="https://www.youtube.com/watch?v=GOJFznzSZhM" class="resource-link" target="_blank">
                <strong>اتم: نبرد غول‌ها</strong>
                <span class="resource-tag">مستند</span>
            </a>
        </div>
    </div>
</div>

<!-- 📰 مقالات -->
<div class="content-section">
    <div class="section-title">
        📰 مقالات علمی <span>۲ منبع</span>
    </div>
    <div class="resources-grid">
        <div class="resource-item">
            <span class="resource-icon">📝</span>
            <a href="https://science.howstuffworks.com/cosmological-redshift.htm" class="resource-link" target="_blank">
                <strong>انتقال به سرخ کیهانی چیست؟</strong>
                <span class="resource-tag">HowStuffWorks</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">🛰️</span>
            <a href="https://www.esa.int/Science_Exploration/Space_Science/What_is_red_shift" class="resource-link" target="_blank">
                <strong>آژانس فضایی اروپا: انتقال به سرخ چیست؟</strong>
                <span class="resource-tag">ESA</span>
            </a>
        </div>
    </div>
</div>

<!-- 🖼️ اینفوگرافیک -->
<div class="content-section">
    <div class="section-title">
        🖼️ اینفوگرافیک آموزشی <span>۱ منبع</span>
    </div>
    <div class="infographic-card">
        <div style="font-size: 3rem; margin-bottom: 10px;">📊</div>
        <a href="https://stsci-opo.org/STScI-01EVSVGBHPK8J8YWETX1TC4Q0K.png" target="_blank">
            🌈 انتقال به سرخ کیهانی چیست؟
        </a>
        <p style="margin-top: 15px; color: rgba(255,255,255,0.9);">
            اینفوگرافیک کامل از پدیده انتقال به سرخ و ارتباط آن با انبساط جهان
        </p>
    </div>
</div>

<!-- 🧪 آشپزخانه کیهان: فعالیت عملی ساخت طیف‌نما -->
<div class="kitchen-card">
    <div style="font-size: 3rem; margin-bottom: 10px;">🧪</div>
    <h2 style="color: #1a3c6e; margin-bottom: 20px;">آشپزخانه کیهان: فعالیت عملی</h2>
    
    <div style="display: flex; flex-wrap: wrap; gap: 30px; align-items: center; justify-content: center; margin: 30px 0;">
        <!-- تصویر راهنمای برش -->
        <div style="flex: 1; min-width: 250px;">
            <img src="../../img/cd-spectroscope-guide.jpg" alt="راهنمای برش برای ساخت طیف‌نما" style="width: 100%; max-width: 350px; border-radius: 16px; box-shadow: 0 8px 20px rgba(0,0,0,0.2); border: 3px solid white;" onerror="this.style.display='none'">
            <p style="margin-top: 10px; color: #1a3c6e; font-size: 0.9rem;">
                <strong>راهنمای برش برای ساخت CD Spectroscope</strong>
            </p>
        </div>
        
        <div style="flex: 2; min-width: 250px;">
            <p style="font-size: 1.1rem; line-height: 1.8; color: #1a3c6e;">
                با استفاده از یک سی‌دی قدیمی و یک لوله مقوایی، یک طیف‌نما بسازید و نور ستاره‌ها را تحلیل کنید!
            </p>
            
            <div style="display: flex; flex-wrap: wrap; gap: 15px; justify-content: center; margin-top: 25px;">
                <a href="https://www.exploratorium.edu/snacks/cd-spectroscope" class="kitchen-link" target="_blank">
                    🧪 دستورالعمل ساخت طیف‌نما
                </a>
                
                <a href="https://www.exploratorium.edu/sites/default/files/snacks/CD-Spectroscope-Cutting-Guide.pdf" class="kitchen-link" target="_blank">
                    📄 دانلود راهنمای برش (PDF)
                </a>
            </div>
            
            <div style="background: rgba(255,255,255,0.5); border-radius: 12px; padding: 15px; margin-top: 20px;">
                <p style="color: #1a3c6e; margin: 0; font-size: 0.95rem;">
                    <strong>📝 نحوه استفاده از راهنمای برش:</strong>
                    <br>
                    ۱. این صفحه را پرینت کنید.<br>
                    ۲. ناحیه مستطیلی سمت چپ را برش بزنید.<br>
                    ۳. دور یک سر لوله مقوایی بپیچید و محکم کنید.<br>
                    ۴. با کاتر، ناحیه سیاه را برای سوراخ دید ببرید.<br>
                    ۵. روی خط منحنی برای شیار سی‌دی برش بزنید.
                </p>
            </div>
        </div>
    </div>
</div>

<!-- دسته‌بندی موضوعی -->
<div class="special-section">
    <div style="display: flex; align-items: center; gap: 10px; margin-bottom: 20px;">
        <span style="font-size: 2rem;">📊</span>
        <h2 style="color: #8b1a1a; margin: 0;">دسته‌بندی موضوعی منابع</h2>
    </div>
    
    <div class="topic-categories">
        <div class="category-card">
            <div class="category-title">
                <span>🚑</span> مفاهیم پایه
            </div>
            <div class="category-items">
                ویدیوهای ۱، ۲، ۳<br>
                اثر داپلر در زندگی روزمره
            </div>
        </div>
        
        <div class="category-card">
            <div class="category-title">
                <span>🔴</span> انتقال به سرخ
            </div>
            <div class="category-items">
                ویدیوهای ۴، ۵، ۶، ۷، ۸، ۱۱<br>
                شبیه‌ساز ردشیفت
            </div>
        </div>
        
        <div class="category-card">
            <div class="category-title">
                <span>🌈</span> طیف‌بینی
            </div>
            <div class="category-items">
                ویدیوهای ۹، ۱۰<br>
                تحلیل طیف ستاره آلتایر
            </div>
        </div>
        
        <div class="category-card">
            <div class="category-title">
                <span>🛠️</span> ابزارهای تعاملی
            </div>
            <div class="category-items">
                ۳ شبیه‌ساز آنلاین<br>
                وبسایت‌های آموزشی
            </div>
        </div>
        
        <div class="category-card">
            <div class="category-title">
                <span>🎬</span> منابع بصری
            </div>
            <div class="category-items">
                مستندها و اینفوگرافیک<br>
                تصاویر و انیمیشن‌ها
            </div>
        </div>
        
        <div class="category-card">
            <div class="category-title">
                <span>🧪</span> آشپزخانه کیهان
            </div>
            <div class="category-items">
                ساخت طیف‌نما با CD<br>
                فعالیت عملی در خانه
            </div>
        </div>
    </div>
</div>

<!-- نقل قول -->
<div style="background: linear-gradient(135deg, #4a0e0e 0%, #8b1a1a 100%); border-radius: 16px; padding: 30px; margin: 30px 0; text-align: center; border: 1px solid #b04a4a;">
    <span style="font-size: 2.5rem; color: white;">🔴</span>
    <p style="font-size: 1.3rem; color: white; font-style: italic; margin: 15px 0;">
        "نور کهکشان‌های دوردست به سرخ می‌گراید؛ گویی جهان به ما می‌گوید که مدام در حال بزرگ‌تر شدن است."
    </p>
    <p style="color: #ffb0b0; font-weight: bold;">- برایان کاکس، فیزیکدان و مجری علمی</p>
</div>

<!-- نکات استفاده -->
<div style="background: #fff0f0; border-radius: 16px; padding: 25px; margin-top: 30px; border-right: 5px solid #8b1a1a;">
    <h3 style="color: #8b1a1a; display: flex; align-items: center; gap: 10px;">
        <span>💡</span> نکات استفاده
    </h3>
    <ul style="color: #8b1a1a; line-height: 1.8; padding-right: 20px;">
        <li>منابع به تفکیک نوع محتوا دسته‌بندی شده‌اند</li>
        <li>مناسب برای آموزش مفاهیم اثر داپلر و انتقال به سرخ در نجوم</li>
        <li>با ابزارهای تعاملی، انتقال به سرخ را به صورت عملی تجربه کنید</li>
        <li>فعالیت ساخت طیف‌نما از کتاب آشپزخانه کیهان را حتماً انجام دهید</li>
        <li>راهنمای برش را پرینت کنید و مطابق دستورالعمل عمل کنید</li>
        <li>اینفوگرافیک انتهای صفحه، دید کلی کاملی از مفهوم ردشیفت ارائه می‌دهد</li>
    </ul>
</div>

<!-- دکمه بازگشت -->
<div style="text-align: center; margin-top: 40px;">
    <a href="/books/cosmoverse/cosmic_library/main_cosmic_library" class="back-button">
        ← بازگشت به کتابخانه کیهانی
    </a>
</div>

</div>
