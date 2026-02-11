---
layout: page
#title: ماجراهای کیهان
#subtitle: سفری شگفت‌انگیز به اعماق کیهان
show_sidebar: false
hero_image: ../../../img/cosmoverse/cosmoverse_logo.png
---

<style>
@import url('https://cdn.jsdelivr.net/gh/rastikerdar/vazir-font@v30.1.0/dist/font-face.css');

.cosmoverse-container {
    font-family: 'Vazir', 'Segoe UI', Tahoma, sans-serif;
    max-width: 1200px;
    margin: 0 auto;
    padding: 20px;
    direction: rtl;
    color: #1a3c6e;
}

/* درباره کتاب */
.about-section {
    background: linear-gradient(135deg, #f0f7ff 0%, #e6f0fa 100%);
    padding: 30px;
    border-radius: 20px;
    margin-bottom: 40px;
    border-right: 6px solid #2c5aa0;
    box-shadow: 0 10px 25px rgba(0,0,0,0.05);
}

.about-section h3 {
    color: #2c5aa0;
    font-size: 1.8rem;
    margin-bottom: 15px;
    border-bottom: 2px solid #c2d9f0;
    padding-bottom: 10px;
}

/* شبکه ۲×۳ فصل‌ها */
.chapters-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 25px;
    margin: 40px 0;
}

.chapter-card {
    background: white;
    border-radius: 16px;
    overflow: hidden;
    box-shadow: 0 8px 20px rgba(44, 90, 160, 0.1);
    transition: all 0.3s ease;
    border: 1px solid #e1ecf4;
    display: flex;
    flex-direction: column;
}

.chapter-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 15px 30px rgba(44, 90, 160, 0.2);
}

.chapter-image {
    width: 100%;
    height: 480px;
    object-fit: cover;
    border-bottom: 3px solid #2c5aa0;
}

.chapter-content {
    padding: 20px;
}

.chapter-title {
    color: #1a3c6e;
    font-size: 1.5rem;
    font-weight: bold;
    margin-bottom: 15px;
    border-bottom: 2px dashed #c2d9f0;
    padding-bottom: 8px;
}

.chapter-sections {
    display: flex;
    flex-direction: column;
    gap: 10px;
}

.section-item {
    display: flex;
    align-items: center;
    gap: 8px;
    color: #2c5aa0;
    text-decoration: none;
    padding: 6px 10px;
    border-radius: 8px;
    transition: background 0.2s;
}

.section-item:hover {
    background: #f0f7ff;
    color: #1a3c6e;
}

.section-icon {
    font-size: 1.2rem;
}

/* کتابخانه کیهانی */
.cosmic-library {
    background: linear-gradient(135deg, #1a3c6e 0%, #2c5aa0 100%);
    padding: 40px;
    border-radius: 20px;
    margin: 50px 0 30px;
    color: white;
    text-align: center;
}

.cosmic-library a {
    color: white;
    text-decoration: none;
    font-size: 1.8rem;
    font-weight: bold;
    display: inline-block;
    padding: 15px 40px;
    background: rgba(255,255,255,0.15);
    border-radius: 50px;
    border: 2px solid rgba(255,255,255,0.3);
    transition: all 0.3s;
}

.cosmic-library a:hover {
    background: rgba(255,255,255,0.25);
    transform: scale(1.05);
}

/* واژه‌نامه */
.glossary {
    background: #f8fafc;
    padding: 30px;
    border-radius: 16px;
    margin-top: 30px;
    border: 1px solid #c2d9f0;
}

.glossary h3 {
    color: #2c5aa0;
    font-size: 1.5rem;
    margin-bottom: 15px;
}

.glossary a {
    color: #1a3c6e;
    text-decoration: none;
    font-size: 1.2rem;
    display: inline-block;
    padding: 8px 25px;
    background: white;
    border-radius: 30px;
    border: 1px solid #2c5aa0;
    transition: all 0.2s;
}

.glossary a:hover {
    background: #2c5aa0;
    color: white;
}

/* ریسپانسیو */
@media (max-width: 900px) {
    .chapters-grid {
        grid-template-columns: repeat(2, 1fr);
    }
}

@media (max-width: 600px) {
    .chapters-grid {
        grid-template-columns: 1fr;
    }
}
</style>

<div class="cosmoverse-container" dir="rtl">

<!-- درباره کتاب -->
<div class="about-section">
    <h3>📘 درباره کتاب</h3>
    <p style="font-size: 1.1rem; line-height: 1.8; color: #1e3a5f;">
        کتاب <strong>«ماجراهای کیهان»</strong> سفری شگفت‌انگیز به دنیای شگفتی‌های کیهان است. 
        این کتاب شما را در ۶ فصل، از بیگ‌بنگ تا اسرار ماده تاریک همراهی می‌کند.
    </p>
</div>

<!-- عنوان فصل‌ها -->
<h2 style="color: #1a3c6e; font-size: 2rem; margin-bottom: 20px; text-align: center;">
    🌌 فصل‌های کتاب
</h2>

<!-- شبکه ۲×۳ فصل‌ها -->
<div class="chapters-grid">

    <!-- فصل ۱: بیگ‌بنگ -->
    <div class="chapter-card">
        <img src="../../../img/cosmoverse/chap1.png" alt="فصل اول: تاریخچه کیهان" class="chapter-image">
        <div class="chapter-content">
            <div class="chapter-title">فصل ۱: تاریخچه کیهان</div>
            <div class="chapter-sections">
                <a href="/books/cosmoverse/ch1/class" class="section-item">📚 کلاس درس</a>
                <a href="/books/cosmoverse/ch1/journey" class="section-item">🚀 سفر با هوماپر</a>
                <a href="/books/cosmoverse/ch1/scientist" class="section-item">👨‍🔬 ملاقات دانشمند</a>
                <a href="/books/cosmoverse/ch1/lab" class="section-item">🔬 آزمایشگاه عملی</a>
                <a href="/books/cosmoverse/ch1/library" class="section-item">📖 کتابخانه کیهانی</a>
            </div>
        </div>
    </div>

    <!-- فصل ۲: مقیاس جهان -->
    <div class="chapter-card">
        <img src="../../../img/cosmoverse/chap2.png" alt="فصل دوم: قانون هابل-لومتر" class="chapter-image">
        <div class="chapter-content">
            <div class="chapter-title">فصل ۲: قانون هابل-لومتر</div>
            <div class="chapter-sections">
                <a href="/books/cosmoverse/ch2/class" class="section-item">📚 کلاس درس</a>
                <a href="/books/cosmoverse/ch2/journey" class="section-item">🚀 سفر با هوماپر</a>
                <a href="/books/cosmoverse/ch2/scientist" class="section-item">👨‍🔬 ملاقات دانشمند</a>
                <a href="/books/cosmoverse/ch2/lab" class="section-item">🔬 آزمایشگاه عملی</a>
                <a href="/books/cosmoverse/ch2/library" class="section-item">📖 کتابخانه کیهانی</a>
            </div>
        </div>
    </div>

    <!-- فصل ۳: انتقال به سرخ -->
    <div class="chapter-card">
        <img src="../../../img/cosmoverse/chap3.png" alt="فصل سوم: سرخ‌گرایی کیهانی" class="chapter-image">
        <div class="chapter-content">
            <div class="chapter-title">فصل ۳: سرخ‌گرایی کیهانی</div>
            <div class="chapter-sections">
                <a href="/books/cosmoverse/ch3/class" class="section-item">📚 کلاس درس</a>
                <a href="/books/cosmoverse/ch3/journey" class="section-item">🚀 سفر با هوماپر</a>
                <a href="/books/cosmoverse/ch3/scientist" class="section-item">👨‍🔬 ملاقات دانشمند</a>
                <a href="/books/cosmoverse/ch3/lab" class="section-item">🔬 آزمایشگاه عملی</a>
                <a href="/books/cosmoverse/ch3/library" class="section-item">📖 کتابخانه کیهانی</a>
            </div>
        </div>
    </div>

    <!-- فصل ۴: نسبیت -->
    <div class="chapter-card">
        <img src="../../../img/cosmoverse/chap4.png" alt="فصل چهارم: گرانش هندسی" class="chapter-image">
        <div class="chapter-content">
            <div class="chapter-title">فصل ۴: گرانش هندسی</div>
            <div class="chapter-sections">
                <a href="/books/cosmoverse/ch4/class" class="section-item">📚 کلاس درس</a>
                <a href="/books/cosmoverse/ch4/journey" class="section-item">🚀 سفر با هوماپر</a>
                <a href="/books/cosmoverse/ch4/scientist" class="section-item">👨‍🔬 ملاقات دانشمند</a>
                <a href="/books/cosmoverse/ch4/lab" class="section-item">🔬 آزمایشگاه عملی</a>
                <a href="/books/cosmoverse/ch4/library" class="section-item">📖 کتابخانه کیهانی</a>
            </div>
        </div>
    </div>

    <!-- فصل ۵: ماده تاریک -->
    <div class="chapter-card">
        <img src="../../../img/cosmoverse/chap5.png" alt="فصل پنجم: ماده تاریک" class="chapter-image">
        <div class="chapter-content">
            <div class="chapter-title">فصل ۵: ماده تاریک</div>
            <div class="chapter-sections">
                <a href="/books/cosmoverse/ch5/class" class="section-item">📚 کلاس درس</a>
                <a href="/books/cosmoverse/ch5/journey" class="section-item">🚀 سفر با هوماپر</a>
                <a href="/books/cosmoverse/ch5/scientist" class="section-item">👨‍🔬 ملاقات دانشمند</a>
                <a href="/books/cosmoverse/ch5/lab" class="section-item">🔬 آزمایشگاه عملی</a>
                <a href="/books/cosmoverse/ch5/library" class="section-item">📖 کتابخانه کیهانی</a>
            </div>
        </div>
    </div>

    <!-- فصل ۶: انرژی تاریک -->
    <div class="chapter-card">
        <img src="../../../img/cosmoverse/chap6.png" alt="فصل ششم: انرژی تاریک" class="chapter-image">
        <div class="chapter-content">
            <div class="chapter-title">فصل ۶: انرژی تاریک</div>
            <div class="chapter-sections">
                <a href="/books/cosmoverse/ch6/class" class="section-item">📚 کلاس درس</a>
                <a href="/books/cosmoverse/ch6/journey" class="section-item">🚀 سفر با هوماپر</a>
                <a href="/books/cosmoverse/ch6/scientist" class="section-item">👨‍🔬 ملاقات دانشمند</a>
                <a href="/books/cosmoverse/ch6/lab" class="section-item">🔬 آزمایشگاه عملی</a>
                <a href="/books/cosmoverse/ch6/library" class="section-item">📖 کتابخانه کیهانی</a>
            </div>
        </div>
    </div>

</div>

<!-- کتابخانه کیهانی -->
<div class="cosmic-library">
    <a href="/books/cosmoverse/cosmic_library/main_cosmic_library">
        🌠 کتابخانه کیهانی (محتوای چندرسانه‌ای)
    </a>
    <p style="color: rgba(255,255,255,0.9); margin-top: 15px; font-size: 1.1rem;">
        ویدیوها، مقالات، آزمون‌ها و بازی‌های تعاملی برای هر فصل
    </p>
</div>

<!-- واژه‌نامه -->
<div class="glossary">
    <h3>📚 واژه‌نامه</h3>
    <p style="margin-bottom: 20px; color: #1e3a5f;">
        فرهنگ‌نامه تخصصی مفاهیم و اصطلاحات کیهان‌شناسی
    </p>
    <a href="/books/cosmoverse/glossary">🔍 جستجو در واژه‌نامه</a>
</div>

</div>