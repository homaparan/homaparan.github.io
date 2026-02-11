---
layout: page
title: کتاب‌های هُماپران دانش
subtitle: آثار مکتوب گروه آموزشی هُماپران دانش
show_sidebar: false
hero_image: ../../img/cmb.jpg
---

<style>
@import url('https://cdn.jsdelivr.net/gh/rastikerdar/vazir-font@v30.1.0/dist/font-face.css');

.books-page {
    font-family: 'Vazir', 'Segoe UI', Tahoma, sans-serif;
    max-width: 1200px;
    margin: 0 auto;
    padding: 20px;
    direction: rtl;
    color: #1a3c6e;
}

/* هدر صفحه */
.books-header {
    background: linear-gradient(135deg, #1e3c5a 0%, #2a4a6e 100%);
    color: white;
    padding: 50px;
    border-radius: 30px;
    margin-bottom: 50px;
    position: relative;
    overflow: hidden;
    box-shadow: 0 15px 30px rgba(26, 60, 110, 0.3);
    text-align: center;
}

.books-header::before {
    content: "📚";
    position: absolute;
    left: 20px;
    top: 20px;
    font-size: 100px;
    opacity: 0.1;
}

.books-header::after {
    content: "✨";
    position: absolute;
    right: 20px;
    bottom: 20px;
    font-size: 100px;
    opacity: 0.1;
}

.books-title {
    font-size: 2.8rem;
    font-weight: bold;
    margin-bottom: 15px;
}

.books-subtitle {
    font-size: 1.2rem;
    opacity: 0.9;
    max-width: 700px;
    margin: 0 auto;
    line-height: 1.8;
}

/* شبکه کتاب‌ها */
.books-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(450px, 1fr));
    gap: 30px;
    margin: 40px 0;
}

.book-card {
    background: white;
    border-radius: 24px;
    overflow: hidden;
    box-shadow: 0 10px 30px rgba(0,0,0,0.05);
    transition: all 0.3s ease;
    border: 1px solid #e1ecf4;
    display: flex;
    flex-direction: row;
    align-items: stretch;
}

.book-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 20px 40px rgba(44, 90, 160, 0.15);
    border-color: #2c5aa0;
}

/* بخش تصویر کتاب */
.book-image-container {
    flex: 0 0 160px;
    background: linear-gradient(135deg, #f0f7ff 0%, #e6f0fa 100%);
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 20px;
    border-left: 1px solid #e1ecf4;
}

.book-image {
    width: 130px;
    height: 180px;
    object-fit: cover;
    border-radius: 12px;
    box-shadow: 0 8px 20px rgba(0,0,0,0.1);
    transition: all 0.3s ease;
}

.book-card:hover .book-image {
    transform: scale(1.05);
    box-shadow: 0 12px 25px rgba(44, 90, 160, 0.2);
}

/* بخش محتوای کتاب */
.book-content {
    flex: 1;
    padding: 25px;
    display: flex;
    flex-direction: column;
}

.book-title {
    font-size: 1.8rem;
    font-weight: bold;
    color: #1a3c6e;
    margin-bottom: 10px;
    line-height: 1.3;
}

.book-subtitle {
    font-size: 0.95rem;
    color: #4a6fa5;
    margin-bottom: 15px;
    display: flex;
    align-items: center;
    gap: 8px;
}

.book-description {
    color: #4a5c6e;
    line-height: 1.7;
    margin-bottom: 20px;
    font-size: 0.95rem;
    flex: 1;
}

/* ویژگی‌های کتاب */
.book-features {
    display: flex;
    flex-wrap: wrap;
    gap: 12px;
    margin-bottom: 20px;
}

.feature-tag {
    background: #eef5ff;
    color: #2c5aa0;
    padding: 5px 15px;
    border-radius: 30px;
    font-size: 0.8rem;
    display: flex;
    align-items: center;
    gap: 6px;
}

/* دکمه مشاهده کتاب */
.book-link {
    display: inline-flex;
    align-items: center;
    gap: 10px;
    background: #2c5aa0;
    color: white;
    padding: 12px 25px;
    border-radius: 30px;
    text-decoration: none;
    font-weight: bold;
    font-size: 0.95rem;
    transition: all 0.2s;
    align-self: flex-start;
    border: 2px solid transparent;
}

.book-link:hover {
    background: white;
    color: #2c5aa0;
    border-color: #2c5aa0;
}

/* بخش کتاب‌های آینده */
.future-books {
    background: linear-gradient(135deg, #f8fafc 0%, #eef5ff 100%);
    border-radius: 30px;
    padding: 40px;
    margin: 60px 0 30px;
    border: 1px dashed #2c5aa0;
    text-align: center;
}

.future-title {
    color: #1a3c6e;
    font-size: 1.5rem;
    margin-bottom: 15px;
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 10px;
}

.future-text {
    color: #4a6fa5;
    font-size: 1rem;
    line-height: 1.8;
}

/* دکمه بازگشت */
.back-button {
    display: inline-flex;
    align-items: center;
    gap: 10px;
    background: #1a3c6e;
    color: white;
    padding: 15px 40px;
    border-radius: 50px;
    text-decoration: none;
    font-weight: bold;
    font-size: 1rem;
    transition: all 0.2s;
    margin-top: 40px;
    border: 2px solid transparent;
}

.back-button:hover {
    background: white;
    color: #1a3c6e;
    border-color: #1a3c6e;
}

/* ریسپانسیو */
@media (max-width: 768px) {
    .books-title {
        font-size: 2rem;
    }
    
    .books-grid {
        grid-template-columns: 1fr;
    }
    
    .book-card {
        flex-direction: column;
    }
    
    .book-image-container {
        flex: 0 0 auto;
        border-left: none;
        border-bottom: 1px solid #e1ecf4;
        padding: 30px;
    }
    
    .book-image {
        width: 150px;
        height: 200px;
    }
}
</style>

<div class="books-page" dir="rtl">

<!-- هدر صفحه -->
<div class="books-header">
    <div class="books-title">📖 کتاب‌های هُماپران دانش</div>
    <div class="books-subtitle">
        مجموعه آثار مکتوب گروه آموزشی هُماپران دانش<br>
        روایت علم به زبان ساده، همراه با تصاویر و فعالیت‌های جذاب
    </div>
</div>

<!-- شبکه کتاب‌ها -->
<div class="books-grid">

    <!-- کتاب ۱: ماجراهای کیهان -->
    <div class="book-card">
        <div class="book-image-container">
            <img src="/img/cosmoverse/cover_half.png" alt="ماجراهای کیهان" class="book-image" onerror="this.src='/img/book-placeholder.jpg'; this.onerror=null;">
        </div>
        <div class="book-content">
            <h2 class="book-title">🌌 ماجراهای کیهان</h2>
            <div class="book-subtitle">
                <span>📅 ۱۴۰۴</span>
                <span>•</span>
                <span>🏢 انتشارات مبتکران</span>
            </div>
            <div class="book-description">
                سفری شگفت‌انگیز از بیگ‌بنگ تا انرژی تاریک. این کتاب شما را در ۶ فصل، با بزرگترین پرسش‌های کیهان‌شناسی آشنا می‌کند. همراه با کتابخانه کیهانی، ویدیوها، آزمون‌ها و فعالیت‌های تعاملی.
            </div>
            <div class="book-features">
                <span class="feature-tag">📘 ۶۸ صفحه</span>
                <span class="feature-tag">🎬 ۶۵+ ویدیو</span>
                <span class="feature-tag">🎮 ۲۰+ تعاملی</span>
                <span class="feature-tag">📊 ۳۰+ اینفوگرافیک</span>
            </div>
            <a href="/books/cosmoverse" class="book-link">
                📖 مطالعه کتاب
                <span style="font-size: 1.2rem;">←</span>
            </a>
        </div>
    </div>

    <!-- کتاب ۲: آشپزخانه کیهان -->
    <div class="book-card">
        <div class="book-image-container">
            <img src="../../img/books/cosmo-kitchen.jpg" alt="آشپزخانه کیهان" class="book-image" onerror="this.src='../../img/book-placeholder.jpg'; this.onerror=null;">
        </div>
        <div class="book-content">
            <h2 class="book-title">🧪 آشپزخانه کیهان</h2>
            <div class="book-subtitle">
                <span>📅 ۱۴۰۴</span>
                <span>•</span>
                <span>🏢 انتشارات مبتکران</span>
            </div>
            <div class="book-description">
                کتاب‌کار همراه ماجرای کیهان! آزمایش‌های علمی ساده با وسایل دور ریختنی، فعالیت‌های عملی و پروژه‌های خلاقانه برای درک عمیق‌تر مفاهیم کیهان‌شناسی. علم را در خانه تجربه کنید!
            </div>
            <div class="book-features">
                <span class="feature-tag">🔬 ۵۰ آزمایش</span>
                <span class="feature-tag">🧪 ۱۲۰ فعالیت</span>
                <span class="feature-tag">📋 برگه‌های کار</span>
                <span class="feature-tag">🏠 مناسب خانه</span>
            </div>
            <a href="/books/cosmo-kitchen" class="book-link">
                📖 مطالعه کتاب
                <span style="font-size: 1.2rem;">←</span>
            </a>
        </div>
    </div>

</div>

<!-- کتاب‌های آینده -->
<div class="future-books">
    <div class="future-title">
        <span>✨</span> کتاب‌های در دست تألیف
    </div>
    <div class="future-text">
        ⚡ سفر در زمان: از اینشتین تا سیاه‌چاله‌ها<br>
        🌍 زمین از نگاه کیهان: اقلیم، محیط زیست و آینده سیاره ما<br>
        🤖 هوش فرازمینی: از افسانه تا علم<br>
    </div>
</div>

<!-- نقل قول -->
<div style="background: #f0f7ff; border-radius: 20px; padding: 30px; margin: 40px 0; text-align: center; border-right: 5px solid #2c5aa0;">
    <span style="font-size: 2.5rem; color: #2c5aa0;">📚</span>
    <p style="font-size: 1.2rem; color: #1a3c6e; font-style: italic; margin: 15px 0; max-width: 700px; margin: 15px auto;">
        "هر کتاب، پنجره‌ای است به سوی دنیایی تازه. ماجرای کیهان و آشپزخانه کیهان، 
        دعوتی‌اند برای سفری بی‌پایان در ژرفای هستی."
    </p>
    <p style="color: #2c5aa0; font-weight: bold;">- گروه هُماپران دانش</p>
</div>

<!-- دکمه بازگشت به صفحه اصلی -->
<div style="text-align: center;">
    <a href="/" class="back-button">
        ← بازگشت به صفحه اصلی
    </a>
</div>

</div>