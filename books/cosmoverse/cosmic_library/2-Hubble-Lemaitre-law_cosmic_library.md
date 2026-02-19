---
layout: page
title: کتابخانه کیهانی - فصل دوم
subtitle: قانون هابل-لومتر | مقیاس جهان | انبساط کیهان
show_sidebar: false
hero_image: ../../img/cmb.jpg
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
    background: linear-gradient(135deg, #0a1a2f 0%, #1a3c6e 100%);
    color: white;
    padding: 40px;
    border-radius: 30px;
    margin-bottom: 40px;
    position: relative;
    overflow: hidden;
    box-shadow: 0 15px 30px rgba(26, 60, 110, 0.3);
}

.chapter-header::before {
    content: "🔭";
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
    border-right: 5px solid #2c5aa0;
    display: flex;
    align-items: center;
    gap: 10px;
}

.section-title span {
    background: #2c5aa0;
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
    background: #eef5ff;
    border-color: #2c5aa0;
    transform: translateX(-5px);
}

.resource-icon {
    font-size: 1.5rem;
    margin-left: 12px;
    color: #2c5aa0;
}

.resource-link {
    color: #1a3c6e;
    text-decoration: none;
    font-size: 0.95rem;
    line-height: 1.6;
    flex: 1;
}

.resource-link:hover {
    color: #2c5aa0;
}

.resource-tag {
    background: #e1ecf4;
    color: #1a3c6e;
    padding: 3px 10px;
    border-radius: 20px;
    font-size: 0.75rem;
    margin-right: 10px;
    white-space: nowrap;
}

/* بخش ویدیوی ویژه */
.featured-video {
    background: linear-gradient(135deg, #f8fafc 0%, #eef5ff 100%);
    border-radius: 20px;
    padding: 30px;
    margin: 30px 0;
    border: 2px solid #2c5aa0;
    position: relative;
    overflow: hidden;
}

.featured-video::before {
    content: "🚀";
    position: absolute;
    left: 20px;
    bottom: 20px;
    font-size: 60px;
    opacity: 0.1;
}

.featured-title {
    color: #1a3c6e;
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
    border-right: 4px solid #ffc107;
}

.featured-quote {
    font-style: italic;
    color: #4a6fa5;
    margin: 15px 0;
    padding-right: 20px;
    border-right: 3px solid #2c5aa0;
}

.featured-link {
    display: inline-flex;
    align-items: center;
    gap: 10px;
    background: #2c5aa0;
    color: white;
    padding: 12px 25px;
    border-radius: 30px;
    text-decoration: none;
    font-weight: bold;
    margin-top: 15px;
    transition: all 0.2s;
}

.featured-link:hover {
    background: #1a3c6e;
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
    background: linear-gradient(135deg, #2c5aa0 0%, #1a3c6e 100%);
    color: white;
    padding: 25px;
    border-radius: 20px;
    text-align: center;
    margin-bottom: 20px;
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

/* بخش‌های ویژه */
.special-section {
    background: linear-gradient(135deg, #f8fafc 0%, #eef5ff 100%);
    border-radius: 20px;
    padding: 30px;
    margin: 40px 0;
    border: 1px dashed #2c5aa0;
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
    border: 1px solid #c2d9f0;
}

.category-title {
    color: #2c5aa0;
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
    background: #1a3c6e;
    color: white;
    text-decoration: none;
    border-radius: 30px;
    transition: all 0.2s;
    border: 2px solid transparent;
}

.back-button:hover {
    background: white;
    color: #1a3c6e;
    border-color: #1a3c6e;
}

/* شمارنده منابع */
.stats-bar {
    display: flex;
    gap: 15px;
    margin-bottom: 30px;
    flex-wrap: wrap;
}

.stat-item {
    background: #eef5ff;
    padding: 8px 20px;
    border-radius: 30px;
    color: #1a3c6e;
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
    <div class="chapter-title">🔭 فصل دوم: قانون هابل-لومتر</div>
    <div class="chapter-subtitle">مقیاس جهان | انبساط کیهان | ثابت هابل</div>
    <div style="display: flex; gap: 15px; margin-top: 20px; flex-wrap: wrap;">
        <span style="background: rgba(255,255,255,0.2); padding: 5px 15px; border-radius: 30px;">📺 ۹ ویدیو</span>
        <span style="background: rgba(255,255,255,0.2); padding: 5px 15px; border-radius: 30px;">🎮 ۱ تعاملی</span>
        <span style="background: rgba(255,255,255,0.2); padding: 5px 15px; border-radius: 30px;">🌐 ۵ وبسایت</span>
        <span style="background: rgba(255,255,255,0.2); padding: 5px 15px; border-radius: 30px;">📚 ۶+ منبع</span>
    </div>
</div>

<!-- آمار سریع -->
<div class="stats-bar">
    <span class="stat-item">📊 مجموع منابع: ۲۱ منبع</span>
    <span class="stat-item">⏱ مناسب برای: ۴ ساعت آموزش</span>
    <span class="stat-item">🎯 سطح: مبتدی تا متوسط</span>
    <span class="stat-item">🔭 کشف: ۱۹۲۹ - ادوین هابل</span>
</div>

<!-- ویدیوی ویژه: آدرس کیهانی ما -->
<div class="featured-video">
    <div class="featured-title">
        <span>🚀</span> ویدیوی ویژه: آدرس کیهانی ما
    </div>
    
    <div style="display: flex; align-items: center; gap: 20px; flex-wrap: wrap;">
        <div style="flex: 1; min-width: 250px;">
            <img src="../../img/cosmic-address.jpg" alt="آدرس کیهانی ما" style="width: 100%; max-width: 300px; border-radius: 16px; box-shadow: 0 8px 20px rgba(0,0,0,0.1);" onerror="this.style.display='none'">
        </div>
        <div style="flex: 2;">
            <div class="featured-description">
                <strong>🎓 عرشه رصدی سفینه تخیل:</strong>
                <p style="margin-top: 10px; color: #1a3c6e;">
                    "عرشه رصدی عظیم سفینه تخیل، جهان را با تمام شکوهش به نمایش گذاشته است. 
                    کوارک در سکوی هدایت ایستاده و مشتاق است دانش‌آموزان را به سفری فراتر از ستاره‌های آشنا ببرد."
                </p>
            </div>
            
            <div class="featured-quote">
                <p>🌟 می‌توانید نرم‌افزار رایگان استلاریوم را دانلود کنید که به شما امکان می‌دهد آزادانه در جهان سفر کنید یا این ویدیو را تماشا کنید:</p>
            </div>
            
            <div style="display: flex; gap: 15px; flex-wrap: wrap;">
                <a href="https://stellarium.org/" class="featured-link" target="_blank">
                    🌌 دانلود نرم‌افزار استلاریوم
                    <span style="font-size: 1.2rem;">←</span>
                </a>
                
                <a href="https://www.youtube.com/watch?v=D4MdwK0Dp5g" class="featured-link" style="background: #ff8c00;" target="_blank">
                    🎬 تماشای ویدیوی آدرس کیهانی
                    <span style="font-size: 1.2rem;">←</span>
                </a>
            </div>
        </div>
    </div>
</div>

<!-- تصاویر ویژه -->
<div class="content-section">
    <div class="section-title">
        🖼️ تصاویر آموزشی <span>۲ تصویر</span>
    </div>
    
    <div class="image-showcase">
        <!-- تصویر موقعیت زمین -->
        <div class="image-card">
            <a href="https://upload.wikimedia.org/wikipedia/commons/8/83/Location_of_Earth_(9x1-English_Annot).jpg" target="_blank">
                <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/8/83/Location_of_Earth_(9x1-English_Annot).jpg/800px-Location_of_Earth_(9x1-English_Annot).jpg" 
                     alt="موقعیت زمین در جهان" 
                     style="width: 100%; border-radius: 12px;">
            </a>
            <div class="image-caption">
                <strong>موقعیت زمین در جهان</strong>
            </div>
            <div class="image-credit">
                شامل ۹ قاب متوالی: زمین، منظومه شمسی درونی، منظومه شمسی بیرونی، ستاره‌های نزدیک، کهکشان راه شیری، گروه محلی، ابرخوشه‌های محلی، لانیاکیا و جهان قابل مشاهده
            </div>
            <div class="image-credit">
                اعتبار: Andrew Z. Colvin
            </div>
            <a href="https://upload.wikimedia.org/wikipedia/commons/8/83/Location_of_Earth_(9x1-English_Annot).jpg" class="image-link" target="_blank">
                🔍 مشاهده تصویر با کیفیت اصلی
            </a>
        </div>
        
        <!-- تصویر نمودار هابل -->
        <div class="image-card">
            <a href="https://commons.wikimedia.org/wiki/File:HubbleTuningFork.jpg" target="_blank">
                <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/1d/HubbleTuningFork.jpg/800px-HubbleTuningFork.jpg" 
                     alt="طرح دسته‌بندی کهکشان‌های هابل" 
                     style="width: 100%; border-radius: 12px;">
            </a>
            <div class="image-caption">
                <strong>طرح دسته‌بندی کهکشان‌های هابل (چنگال هابل)</strong>
            </div>
            <div class="image-credit">
                ادوین هابل، ستاره‌شناس آمریکایی، این طرح دسته‌بندی کهکشان‌ها را در سال ۱۹۲۶ ارائه کرد. اگرچه این طرح، که به نمودار چنگال هابل نیز معروف است، امروزه تا حدودی ساده‌انگارانه تلقی می‌شود، اما اصول اولیه آن همچنان معتبر است.
            </div>
            <div style="direction: ltr; text-align: left; margin-top: 10px; font-family: monospace;">
                <strong>E0 E3 E5 E7 S0</strong><br>
                <strong>Sa Sb Sc</strong><br>
                <strong>SBa SBb SBc</strong>
            </div>
            <a href="https://commons.wikimedia.org/wiki/File:HubbleTuningFork.jpg" class="image-link" target="_blank">
                🔍 مشاهده تصویر اصلی در ویکی‌مدیا
            </a>
        </div>
    </div>
</div>

<!-- 📺 ویدیوها -->
<div class="content-section">
    <div class="section-title">
        📺 ویدیوهای آموزشی <span>۹ منبع</span>
    </div>
    <div class="resources-grid">
        <!-- ردیف ۱ -->
        <div class="resource-item">
            <span class="resource-icon">📏</span>
            <a href="https://www.youtube.com/watch?v=WYQ3O8U6SMY" class="resource-link" target="_blank">
                <strong>ما در مقیاس جهان چقدر کوچک هستیم؟</strong>
                <span class="resource-tag">مقیاس</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">📐</span>
            <a href="https://www.khanacademy.org/science/cosmology-and-astronomy/universe-scale-topic/scale-earth-galaxy-tutorial/v/scale-of-the-large" class="resource-link" target="_blank">
                <strong>مقیاس بزرگ - آکادمی خان</strong>
                <span class="resource-tag">آکادمی خان</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">🚀</span>
            <a href="https://www.youtube.com/watch?v=H14TSlXuzcQ" class="resource-link" target="_blank">
                <strong>سفر حماسی از زمین تا لبه جهان</strong>
                <span class="resource-tag">مقیاس</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">🌍</span>
            <a href="https://www.youtube.com/watch?v=bj-Xvh00c0Y" class="resource-link" target="_blank">
                <strong>آدرس کیهانی ما چیست؟</strong>
                <span class="resource-tag">مقیاس</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">📊</span>
            <a href="https://www.youtube.com/watch?v=1V9wVmO0Tfg" class="resource-link" target="_blank">
                <strong>قانون هابل - مقیاس جهان</strong>
                <span class="resource-tag">هابل</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">📈</span>
            <a href="https://www.youtube.com/watch?v=fGkN30FXcz4" class="resource-link" target="_blank">
                <strong>قانون هابل</strong>
                <span class="resource-tag">هابل</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">🌌</span>
            <a href="https://www.youtube.com/watch?v=8MOHzDK38pE" class="resource-link" target="_blank">
                <strong>قانون هابل: جهان چقدر بزرگ است؟</strong>
                <span class="resource-tag">هابل</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">🏛️</span>
            <a href="https://www.rmg.co.uk/schools-communities/teacher-resources/hubbles-law" class="resource-link" target="_blank">
                <strong>قانون هابل</strong>
                <span class="resource-tag">منابع معلم</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">💫</span>
            <a href="https://www.youtube.com/watch?v=wEf_2bnNdFo" class="resource-link" target="_blank">
                <strong>انبساط جهان!</strong>
                <span class="resource-tag">هابل</span>
            </a>
        </div>
    </div>
</div>

<!-- 🎮 تعاملی ویژه -->
<div class="content-section">
    <div class="section-title">
        🎮 ابزارهای تعاملی <span>۱ منبع</span>
    </div>
    <div class="interactive-card">
        <div style="font-size: 3rem; margin-bottom: 10px;">🪐</div>
        <a href="https://htwins.net/scale2/" target="_blank">
            🌠 مقیاس جهان (The Scale of the Universe)
        </a>
        <p style="margin-top: 15px; color: rgba(255,255,255,0.9);">
            تجربه‌ای شگفت‌انگیز از کوچک‌ترین تا بزرگ‌ترین مقیاس‌های جهان
        </p>
    </div>
</div>

<!-- 🌐 وبسایت‌ها -->
<div class="content-section">
    <div class="section-title">
        🌐 وبسایت‌های مرجع <span>۵ منبع</span>
    </div>
    <div class="resources-grid">
        <div class="resource-item">
            <span class="resource-icon">🛰️</span>
            <a href="https://www.nasa.gov/content/discoveries-hubbles-deep-fields" class="resource-link" target="_blank">
                <strong>ناسا - تلسکوپ فضایی هابل</strong>
                <span class="resource-tag">ناسا</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">👨‍🏫</span>
            <a href="https://spark.iop.org/episode-704-expanding-universe" class="resource-link" target="_blank">
                <strong>منابع معلمان - انبساط جهان</strong>
                <span class="resource-tag">IOP</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">📏</span>
            <a href="https://chandra.si.edu/scale/" class="resource-link" target="_blank">
                <strong>مقیاس و فاصله</strong>
                <span class="resource-tag">چاندرا</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">📚</span>
            <a href="https://bhp-public.oerproject.com/" class="resource-link" target="_blank">
                <strong>پروژه تاریخ بزرگ</strong>
                <span class="resource-tag">BHP</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">🔭</span>
            <a href="https://science.nasa.gov/astrophysics/focus-areas/what-powered-the-big-bang" class="resource-link" target="_blank">
                <strong>خلاصه ناسا از آخرین اکتشافات</strong>
                <span class="resource-tag">ناسا</span>
            </a>
        </div>
    </div>
</div>

<!-- 🎬 مستندها -->
<div class="content-section">
    <div class="section-title">
        🎬 مستندهای علمی <span>۲ منبع</span>
    </div>
    <div class="resources-grid">
        <div class="resource-item">
            <span class="resource-icon">🎞️</span>
            <a href="https://www.youtube.com/watch?v=68tpCpDOsyA" class="resource-link" target="_blank">
                <strong>سفر به لبه جهان</strong>
                <span class="resource-tag">مستند</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">🎞️</span>
            <a href="https://topdocumentaryfilms.com/everything-and-nothing/" class="resource-link" target="_blank">
                <strong>همه چیز و هیچ چیز</strong>
                <span class="resource-tag">مستند</span>
            </a>
        </div>
    </div>
</div>

<!-- 📚 کتاب‌ها -->
<div class="content-section">
    <div class="section-title">
        📚 کتاب‌های تخصصی <span>۱ منبع</span>
    </div>
    <div class="resources-grid">
        <div class="resource-item">
            <span class="resource-icon">📖</span>
            <a href="https://archive.org/details/daywefounduniver00bart" class="resource-link" target="_blank">
                <strong>روزی که جهان را پیدا کردیم</strong>
                <span class="resource-tag">آرشیو</span>
            </a>
        </div>
    </div>
</div>

<!-- 📰 مقالات -->
<div class="content-section">
    <div class="section-title">
        📰 مقالات علمی <span>۳ منبع</span>
    </div>
    <div class="resources-grid">
        <div class="resource-item">
            <span class="resource-icon">📰</span>
            <a href="https://www.universetoday.com/90862/the-expanding-universe-credit-to-hubble-or-lemaitre/" class="resource-link" target="_blank">
                <strong>جهان در حال انبساط: از هابل و لومتر</strong>
                <span class="resource-tag">Universe Today</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">📰</span>
            <a href="https://www.space.com/52-the-expanding-universe-from-the-big-bang-to-today.html" class="resource-link" target="_blank">
                <strong>جهان در حال انبساط ما: سن، تاریخ و حقایق دیگر</strong>
                <span class="resource-tag">Space.com</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">📰</span>
            <a href="https://www.space.fm/astronomy/starsgalaxies/hubbleslawconstant.html" class="resource-link" target="_blank">
                <strong>قانون هابل و ثابت هابل</strong>
                <span class="resource-tag">Space FM</span>
            </a>
        </div>
    </div>
</div>

<!-- ❓ آزمون‌ها -->
<div class="content-section">
    <div class="section-title">
        ❓ آزمون‌های تعاملی <span>۳ منبع</span>
    </div>
    <div class="resources-grid">
        <div class="resource-item">
            <span class="resource-icon">📝</span>
            <a href="https://www.stem.org.uk/elibrary/resource/31663" class="resource-link" target="_blank">
                <strong>سن جهان</strong>
                <span class="resource-tag">STEM</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">📝</span>
            <a href="https://quizizz.com/admin/quiz/5bf2a43e5be548001a37f0c4/astronomy-3-3-hubbles-law" class="resource-link" target="_blank">
                <strong>قانون هابل-لومتر</strong>
                <span class="resource-tag">Quizizz</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">📝</span>
            <a href="https://study.com/academy/practice/quiz-worksheet-hubble-s-law-hubble-s-constant.html" class="resource-link" target="_blank">
                <strong>قانون هابل و ثابت هابل</strong>
                <span class="resource-tag">Study.com</span>
            </a>
        </div>
    </div>
</div>

<!-- 🎮 بازی‌ها و فعالیت‌ها -->
<div class="content-section">
    <div class="section-title">
        🎮 بازی‌ها و فعالیت‌ها <span>۱ منبع</span>
    </div>
    <div class="resources-grid">
        <div class="resource-item">
            <span class="resource-icon">🎲</span>
            <a href="https://www.nisenet.org/sites/default/files/exsci_space_expanding_sign.pdf" class="resource-link" target="_blank">
                <strong>جهان در حال انبساط</strong>
                <span class="resource-tag">فعالیت</span>
            </a>
        </div>
    </div>
</div>

<!-- دسته‌بندی موضوعی -->
<div class="special-section">
    <div style="display: flex; align-items: center; gap: 10px; margin-bottom: 20px;">
        <span style="font-size: 2rem;">📊</span>
        <h2 style="color: #1a3c6e; margin: 0;">دسته‌بندی موضوعی منابع</h2>
    </div>
    
    <div class="topic-categories">
        <div class="category-card">
            <div class="category-title">
                <span>📏</span> مقیاس و اندازه
            </div>
            <div class="category-items">
                ویدیوهای ۱، ۲، ۳، ۴<br>
                ابزار تعاملی: مقیاس جهان
            </div>
        </div>
        
        <div class="category-card">
            <div class="category-title">
                <span>📊</span> قانون هابل
            </div>
            <div class="category-items">
                ویدیوهای ۵، ۶، ۷، ۸، ۹<br>
                مقالات و آزمون‌ها
            </div>
        </div>
        
        <div class="category-card">
            <div class="category-title">
                <span>🔭</span> ابزارهای تعاملی
            </div>
            <div class="category-items">
                مقیاس جهان (The Scale)<br>
                نرم‌افزار استلاریوم
            </div>
        </div>
        
        <div class="category-card">
            <div class="category-title">
                <span>🎬</span> مستندهای بصری
            </div>
            <div class="category-items">
                سفر به لبه جهان<br>
                همه چیز و هیچ چیز
            </div>
        </div>
        
        <div class="category-card">
            <div class="category-title">
                <span>👨‍🏫</span> منابع آموزشی
            </div>
            <div class="category-items">
                وبسایت‌ها، مقالات<br>
                آزمون‌ها و فعالیت‌ها
            </div>
        </div>
    </div>
</div>

<!-- نکات استفاده -->
<div style="background: #fff9e6; border-radius: 16px; padding: 25px; margin-top: 30px; border-right: 5px solid #ffc107;">
    <h3 style="color: #856404; display: flex; align-items: center; gap: 10px;">
        <span>💡</span> نکات استفاده
    </h3>
    <ul style="color: #856404; line-height: 1.8; padding-right: 20px;">
        <li>منابع به تفکیک نوع محتوا دسته‌بندی شده‌اند</li>
        <li>مناسب برای آموزش مفاهیم مقیاس جهان و انبساط کیهانی</li>
        <li>ابزار تعاملی "مقیاس جهان" را حتماً تجربه کنید</li>
        <li>نرم‌افزار رایگان استلاریوم را دانلود کنید و در جهان سفر کنید</li>
        <li>تصویر موقعیت زمین در جهان، درک عمیقی از جایگاه ما در کیهان به شما می‌دهد</li>
        <li>نمودار چنگال هابل، طبقه‌بندی کهکشان‌ها را به زیبایی نشان می‌دهد</li>
    </ul>
</div>

<!-- دکمه بازگشت -->
<div style="text-align: center; margin-top: 40px;">
    <a href="/books/cosmoverse/cosmic_library/main_cosmic_library" class="back-button">
        ← بازگشت به کتابخانه کیهانی
    </a>
</div>

</div>