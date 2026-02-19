---
layout: page
title: کتابخانه کیهانی - فصل ششم
subtitle: انرژی تاریک | انبساط شتاب‌دار | ثابت کیهان‌شناختی
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
    background: linear-gradient(135deg, #1e2a47 0%, #0f1a2f 100%);
    color: white;
    padding: 40px;
    border-radius: 30px;
    margin-bottom: 40px;
    position: relative;
    overflow: hidden;
    box-shadow: 0 15px 30px rgba(15, 26, 47, 0.4);
}

.chapter-header::before {
    content: "⚡";
    position: absolute;
    left: 20px;
    top: 20px;
    font-size: 80px;
    opacity: 0.15;
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
    color: #0f1a2f;
    font-size: 1.8rem;
    margin-bottom: 25px;
    padding-right: 15px;
    border-right: 5px solid #4a6b9f;
    display: flex;
    align-items: center;
    gap: 10px;
}

.section-title span {
    background: #4a6b9f;
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
    background: #e8f0fe;
    border-color: #4a6b9f;
    transform: translateX(-5px);
}

.resource-icon {
    font-size: 1.5rem;
    margin-left: 12px;
    color: #4a6b9f;
}

.resource-link {
    color: #0f1a2f;
    text-decoration: none;
    font-size: 0.95rem;
    line-height: 1.6;
    flex: 1;
}

.resource-link:hover {
    color: #4a6b9f;
}

.resource-tag {
    background: #e1ecf4;
    color: #0f1a2f;
    padding: 3px 10px;
    border-radius: 20px;
    font-size: 0.75rem;
    margin-right: 10px;
    white-space: nowrap;
}

/* بخش‌های ویژه */
.special-section {
    background: linear-gradient(135deg, #f0f4fc 0%, #e6ecf8 100%);
    border-radius: 20px;
    padding: 30px;
    margin: 40px 0;
    border: 1px dashed #4a6b9f;
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
    color: #0f1a2f;
    font-size: 1.2rem;
    font-weight: bold;
    margin-bottom: 10px;
    display: flex;
    align-items: center;
    gap: 8px;
}

.category-items {
    color: #4a6b9f;
    font-size: 0.9rem;
    line-height: 1.8;
}

/* دکمه بازگشت */
.back-button {
    display: inline-block;
    margin-top: 30px;
    padding: 12px 30px;
    background: #0f1a2f;
    color: white;
    text-decoration: none;
    border-radius: 30px;
    transition: all 0.2s;
    border: 2px solid transparent;
}

.back-button:hover {
    background: white;
    color: #0f1a2f;
    border-color: #0f1a2f;
}

/* شمارنده منابع */
.stats-bar {
    display: flex;
    gap: 15px;
    margin-bottom: 30px;
    flex-wrap: wrap;
}

.stat-item {
    background: #e6ecf8;
    padding: 8px 20px;
    border-radius: 30px;
    color: #0f1a2f;
    font-size: 0.9rem;
    display: flex;
    align-items: center;
    gap: 5px;
}

/* کارت تعاملی ویژه */
.interactive-card {
    background: linear-gradient(135deg, #2c3e5c 0%, #1a2a44 100%);
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

/* کارت کتاب */
.book-card {
    background: linear-gradient(135deg, #ffd89b 0%, #f7b733 100%);
    color: #0f1a2f;
    padding: 25px;
    border-radius: 20px;
    text-align: center;
    margin-bottom: 20px;
}

.book-card a {
    color: #0f1a2f;
    font-weight: bold;
    text-decoration: none;
    font-size: 1.2rem;
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
    <div class="chapter-title">⚡ فصل ششم: انرژی تاریک</div>
    <div class="chapter-subtitle">انبساط شتاب‌دار | ثابت کیهان‌شناختی</div>
    <div style="display: flex; gap: 15px; margin-top: 20px; flex-wrap: wrap;">
        <span style="background: rgba(255,255,255,0.2); padding: 5px 15px; border-radius: 30px;">📺 ۱۱ ویدیو</span>
        <span style="background: rgba(255,255,255,0.2); padding: 5px 15px; border-radius: 30px;">🎮 ۲ تعاملی</span>
        <span style="background: rgba(255,255,255,0.2); padding: 5px 15px; border-radius: 30px;">🌐 ۷ وبسایت</span>
        <span style="background: rgba(255,255,255,0.2); padding: 5px 15px; border-radius: 30px;">📚 ۱ کتاب</span>
    </div>
</div>


<!-- اینفوگرافیک ترکیب جهان - فصل ۶ (انرژی تاریک) -->
<div style="background: linear-gradient(135deg, #1a2a44 0%, #0f1a2f 100%); border-radius: 20px; padding: 30px; margin: 30px 0; text-align: center; color: white; border: 1px solid #4a6b9f;">
    <h3 style="color: white; font-size: 1.8rem; margin-bottom: 20px;">⚡ ترکیب جهان: انرژی تاریک</h3>
    
    <!-- نمودار اصلی -->
    <div style="display: flex; justify-content: center; align-items: center; gap: 40px; flex-wrap: wrap; margin-bottom: 30px;">
        <!-- انرژی تاریک (۶۸٪) - برجسته‌تر -->
        <div style="text-align: center;">
            <div style="width: 160px; height: 160px; border-radius: 50%; background: linear-gradient(135deg, #4a6b9f 0%, #2c4a7a 100%); margin: 0 auto; display: flex; align-items: center; justify-content: center; font-size: 2.8rem; font-weight: bold; color: white; border: 3px solid #ffd966; box-shadow: 0 0 30px #ffd966;">۶۸٪</div>
            <p style="margin-top: 15px; font-weight: bold; color: #ffd966;">⚡ انرژی تاریک</p>
        </div>
        
        <!-- ماده تاریک (۲۷٪) -->
        <div style="text-align: center;">
            <div style="width: 100px; height: 100px; border-radius: 50%; background: #2c3e5c; margin: 0 auto; display: flex; align-items: center; justify-content: center; font-size: 2rem; font-weight: bold; color: white; box-shadow: 0 8px 15px rgba(0,0,0,0.3);">۲۷٪</div>
            <p style="margin-top: 15px; font-weight: bold; color: #a0c0ff;">ماده تاریک</p>
        </div>
        
        <!-- ماده معمولی (۵٪) -->
        <div style="text-align: center;">
            <div style="width: 80px; height: 80px; border-radius: 50%; background: #5a7ea0; margin: 0 auto; display: flex; align-items: center; justify-content: center; font-size: 1.5rem; font-weight: bold; color: white; box-shadow: 0 8px 15px rgba(0,0,0,0.3);">۵٪</div>
            <p style="margin-top: 15px; font-weight: bold; color: #a0c0ff;">ماده معمولی</p>
        </div>
    </div>
    
    <!-- توضیح تکمیلی -->
    <div style="margin-top: 25px; padding: 15px; background: rgba(74, 107, 159, 0.3); border-radius: 12px; font-size: 0.95rem; color: #ffd966;">
        <span style="font-weight: bold;">⚡ واقعیت شگفت‌انگیز:</span> انرژی تاریک نیروی اسرارآمیزی است که باعث انبساط شتاب‌دار جهان می‌شود. حدود ۶۸٪ از جهان از این انرژی ناشناخته تشکیل شده است!
    </div>
</div>

<!-- آمار سریع -->
<div class="stats-bar">
    <span class="stat-item">📊 مجموع منابع: ۲۳ منبع</span>
    <span class="stat-item">⏱ مناسب برای: ۶ ساعت آموزش</span>
    <span class="stat-item">🎯 سطح: پیشرفته</span>
    <span class="stat-item">⚡ کشف: ۱۹۹۸ - پرلموتر، ریس، اشمیت</span>
</div>

<!-- 📺 ویدیوها -->
<div class="content-section">
    <div class="section-title">
        📺 ویدیوهای آموزشی <span>۱۱ منبع</span>
    </div>
    <div class="resources-grid">
        <!-- مفاهیم پایه -->
        <div class="resource-item">
            <span class="resource-icon">🌀</span>
            <a href="https://www.youtube.com/watch?v=5LW_2J2qs0Y" class="resource-link" target="_blank">
                <strong>سوی تاریک جهان - برایان گرین</strong>
                <span class="resource-tag">پیشرفته</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">⚡</span>
            <a href="https://www.youtube.com/watch?v=clA9WRZA8K8" class="resource-link" target="_blank">
                <strong>انرژی تاریک چیست؟</strong>
                <span class="resource-tag">پایه</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">🌑</span>
            <a href="https://www.youtube.com/watch?v=QAa2O_8wBUQ&t=5s" class="resource-link" target="_blank">
                <strong>ماده تاریک و انرژی تاریک چیست؟</strong>
                <span class="resource-tag">پایه</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">🛰️</span>
            <a href="https://www.youtube.com/watch?v=YQq0VdJApzU" class="resource-link" target="_blank">
                <strong>گشودن اسرار انرژی تاریک با دابلیو‌فرست ناسا</strong>
                <span class="resource-tag">پیشرفته</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">❓</span>
            <a href="https://www.youtube.com/watch?v=wnSVBLXaoO8" class="resource-link" target="_blank">
                <strong>انرژی تاریک از چه ساخته شده است؟ کوئینتسنس؟ ثابت کیهان‌شناختی؟</strong>
                <span class="resource-tag">پیشرفته</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">📚</span>
            <a href="https://www.youtube.com/watch?v=gzLM6ltw3l0" class="resource-link" target="_blank">
                <strong>انرژی تاریک، کیهان‌شناسی بخش ۲: دوره فشرده نجوم</strong>
                <span class="resource-tag">پایه</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">🌌</span>
            <a href="https://www.youtube.com/watch?v=xZTb6sfHEX8" class="resource-link" target="_blank">
                <strong>آیا جهان برای همیشه منبسط خواهد شد؟</strong>
                <span class="resource-tag">سرنوشت</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">❓</span>
            <a href="https://www.youtube.com/watch?v=-4PayaEgEZc" class="resource-link" target="_blank">
                <strong>چرا جهان به انرژی تاریک نیاز دارد؟</strong>
                <span class="resource-tag">سرنوشت</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">🔮</span>
            <a href="https://www.youtube.com/watch?v=RUE_LUqcTvM" class="resource-link" target="_blank">
                <strong>انرژی تاریک واقعاً چه می‌کند؟</strong>
                <span class="resource-tag">سرنوشت</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">⭐</span>
            <a href="https://www.youtube.com/watch?v=uBbxXNhZ78c" class="resource-link" target="_blank">
                <strong>نیل دگراس تایسون: ماده تاریک چیست؟ انرژی تاریک چیست؟</strong>
                <span class="resource-tag">پایه</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">🗺️</span>
            <a href="https://www.youtube.com/watch?v=fKFBdibfoZM" class="resource-link" target="_blank">
                <strong>نقشه‌برداری از جهان: انرژی تاریک، سیاه‌چاله‌ها و گرانش</strong>
                <span class="resource-tag">پیشرفته</span>
            </a>
        </div>
    </div>
</div>

<!-- 🎮 تعاملی و اینفوگرافیک‌ها -->
<div class="content-section">
    <div class="section-title">
        🎮 تعاملی و اینفوگرافیک‌ها <span>۲ منبع</span>
    </div>
    <div class="interactive-card">
        <div style="font-size: 2.5rem; margin-bottom: 10px;">🛰️</div>
        <a href="https://roman.gsfc.nasa.gov/dark_energy.html" target="_blank">
            🌌 شبیه‌ساز انرژی تاریک - تلسکوپ رومن ناسا
        </a>
        <p style="margin-top: 15px; color: rgba(255,255,255,0.9);">
            مأموریت بعدی ناسا برای کشف ماهیت انرژی تاریک
        </p>
    </div>
    
    <div class="resources-grid" style="margin-top: 20px;">
        <div class="resource-item">
            <span class="resource-icon">📊</span>
            <a href="https://futurism.com/dark-matter-and-dark-energy-explained-infographic" class="resource-link" target="_blank">
                <strong>ماده تاریک و انرژی تاریک توضیح داده شده (اینفوگرافیک)</strong>
                <span class="resource-tag">تصویری</span>
            </a>
        </div>
    </div>
</div>

<!-- 🌐 وبسایت‌ها و مقالات -->
<div class="content-section">
    <div class="section-title">
        🌐 وبسایت‌ها و مقالات <span>۷ منبع</span>
    </div>
    <div class="resources-grid">
        <div class="resource-item">
            <span class="resource-icon">📰</span>
            <a href="https://www.forbes.com/sites/startswithabang/2019/01/04/the-five-ways-the-universe-might-end/?sh=2120c51b3496" class="resource-link" target="_blank">
                <strong>پنج راهی که جهان ممکن است به پایان برسد</strong>
                <span class="resource-tag">فوربس</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">📚</span>
            <a href="https://futurism.com/tags/dark-energy" class="resource-link" target="_blank">
                <strong>مقالات و اخبار مختلف درباره انرژی تاریک</strong>
                <span class="resource-tag">Futurism</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">🔮</span>
            <a href="https://futurism.com/four-ways-the-universe-could-end" class="resource-link" target="_blank">
                <strong>چهار راهی که جهان ما ممکن است پایان یابد</strong>
                <span class="resource-tag">Futurism</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">🚀</span>
            <a href="https://science.nasa.gov/astrophysics/focus-areas/what-is-dark-energy/" class="resource-link" target="_blank">
                <strong>انرژی تاریک، ماده تاریک - ناسا</strong>
                <span class="resource-tag">ناسا</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">🔭</span>
            <a href="https://hubblesite.org/contents/articles/dark-energy" class="resource-link" target="_blank">
                <strong>شتاب‌گیری انبساط جهان</strong>
                <span class="resource-tag">هابل</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">🌍</span>
            <a href="https://www.nationalgeographic.com/science/article/dark-matter" class="resource-link" target="_blank">
                <strong>ماده تاریک و انرژی تاریک - نشنال جئوگرافیک</strong>
                <span class="resource-tag">نشنال جئوگرافیک</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">🏛️</span>
            <a href="https://www.smithsonianmag.com/science-nature/dark-energy-the-biggest-mystery-in-the-universe-9482130/" class="resource-link" target="_blank">
                <strong>انرژی تاریک: بزرگترین رمز و راز جهان</strong>
                <span class="resource-tag">اسمیتسونیان</span>
            </a>
        </div>
    </div>
</div>

<!-- 📚 کتاب‌ها -->
<div class="content-section">
    <div class="section-title">
        📚 کتاب‌های تخصصی <span>۱ منبع</span>
    </div>
    <div class="book-card">
        <div style="font-size: 2.5rem; margin-bottom: 10px;">📘</div>
        <a href="https://www.learner.org/wp-content/uploads/2019/02/physics-for-21st-century-dark-energy-online-textbook.pdf" target="_blank">
            فیزیک برای قرن ۲۱: انرژی تاریک - کتاب درسی آنلاین
        </a>
        <p style="margin-top: 15px; color: #0f1a2f;">
            کتاب جامع و رایگان از پروژه فیزیک قرن ۲۱
        </p>
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
            <a href="https://www.youtube.com/watch?v=kMVOE3UEMqE" class="resource-link" target="_blank">
                <strong>انرژی تاریک: بزرگترین رمز و راز در جهان</strong>
                <span class="resource-tag">مستند</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">📺</span>
            <a href="https://topdocumentaryfilms.com/most-of-the-universe-is-missing/" class="resource-link" target="_blank">
                <strong>بیشتر جهان گمشده است</strong>
                <span class="resource-tag">مستند</span>
            </a>
        </div>
    </div>
</div>

<!-- ❓ آزمون‌ها -->
<div class="content-section">
    <div class="section-title">
        ❓ آزمون‌های تعاملی <span>۲ منبع</span>
    </div>
    <div class="resources-grid">
        <div class="resource-item">
            <span class="resource-icon">📝</span>
            <a href="https://quizizz.com/admin/quiz/5b5250bc84d6e7001a09144a/dark-energy-cosmology-part-2?fromSearch=true&source=" class="resource-link" target="_blank">
                <strong>آزمون انرژی تاریک</strong>
                <span class="resource-tag">Quizizz</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">❓</span>
            <a href="https://www.funtrivia.com/trivia-quiz/SciTech/The-Mystery-of-Dark-Matter-and-Dark-Energy-366588.html" class="resource-link" target="_blank">
                <strong>رمز و راز انرژی تاریک</strong>
                <span class="resource-tag">FunTrivia</span>
            </a>
        </div>
    </div>
</div>

<!-- دسته‌بندی موضوعی -->
<div class="special-section">
    <div style="display: flex; align-items: center; gap: 10px; margin-bottom: 20px;">
        <span style="font-size: 2rem;">📊</span>
        <h2 style="color: #0f1a2f; margin: 0;">دسته‌بندی موضوعی منابع</h2>
    </div>
    
    <div class="topic-categories">
        <div class="category-card">
            <div class="category-title">
                <span>📘</span> مفاهیم پایه
            </div>
            <div class="category-items">
                ویدیوهای ۲، ۳، ۶، ۱۰<br>
                آشنایی با انرژی تاریک
            </div>
        </div>
        
        <div class="category-card">
            <div class="category-title">
                <span>🔬</span> تحقیقات پیشرفته
            </div>
            <div class="category-items">
                ویدیوهای ۴، ۵، ۱۱<br>
                مأموریت‌های فضایی
            </div>
        </div>
        
        <div class="category-card">
            <div class="category-title">
                <span>🌌</span> سرنوشت جهان
            </div>
            <div class="category-items">
                ویدیوهای ۷، ۸، ۹<br>
                مقالات ۱ و ۳
            </div>
        </div>
        
        <div class="category-card">
            <div class="category-title">
                <span>🛠️</span> ابزارهای آموزشی
            </div>
            <div class="category-items">
                شبیه‌ساز رومن<br>
                اینفوگرافیک‌ها
            </div>
        </div>
        
        <div class="category-card">
            <div class="category-title">
                <span>🎬</span> مستندهای علمی
            </div>
            <div class="category-items">
                ۲ مستند برتر<br>
                کاوش در بزرگترین اسرار
            </div>
        </div>
    </div>
</div>

<!-- نقل قول -->
<div style="background: #0f1a2f; border-radius: 16px; padding: 30px; margin: 30px 0; text-align: center; border: 1px solid #4a6b9f;">
    <span style="font-size: 2.5rem; color: white;">⚡</span>
    <p style="font-size: 1.3rem; color: white; font-style: italic; margin: 15px 0;">
        "انرژی تاریک نه تنها بزرگترین راز کیهان‌شناسی مدرن است، 
        بلکه شاید بزرگترین راز در تمام فیزیک باشد."
    </p>
    <p style="color: #a0b8d0; font-weight: bold;">- آدام ریس، برنده جایزه نوبل فیزیک ۲۰۱۱</p>
</div>


<!-- نکات استفاده -->
<div style="background: #e6ecf8; border-radius: 16px; padding: 25px; margin-top: 30px; border-right: 5px solid #4a6b9f;">
    <h3 style="color: #0f1a2f; display: flex; align-items: center; gap: 10px;">
        <span>💡</span> نکات استفاده
    </h3>
    <ul style="color: #0f1a2f; line-height: 1.8; padding-right: 20px;">
        <li>منابع به تفکیک مفاهیم پایه، تحقیقات پیشرفته و سرنوشت جهان دسته‌بندی شده‌اند</li>
        <li>مناسب برای درک یکی از بزرگترین کشفیات نجومی قرن بیستم</li>
        <li>شبیه‌ساز تلسکوپ رومن ناسا را حتماً ببینید - آینده تحقیقات انرژی تاریک</li>
        <li>کتاب درسی آنلاین فیزیک قرن ۲۱ منبعی عالی برای مطالعه عمیق است</li>
        <li>مستند "بیشتر جهان گمشده است" از BBC، نمای کاملی از مسئله ارائه می‌دهد</li>
    </ul>
</div>

<!-- دکمه بازگشت -->
<div style="text-align: center; margin-top: 40px;">
    <a href="/books/cosmoverse/cosmic_library/main_cosmic_library" class="back-button">
        ← بازگشت به کتابخانه کیهانی
    </a>
</div>

</div>