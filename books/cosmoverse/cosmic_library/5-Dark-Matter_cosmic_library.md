---
layout: page
title: کتابخانه کیهانی - فصل پنجم
subtitle: ماده تاریک | جرم گمشده | عدسی گرانشی
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
    background: linear-gradient(135deg, #0f0f1f 0%, #1a1a2e 100%);
    color: white;
    padding: 40px;
    border-radius: 30px;
    margin-bottom: 40px;
    position: relative;
    overflow: hidden;
    box-shadow: 0 15px 30px rgba(26, 26, 46, 0.4);
}

.chapter-header::before {
    content: "🌑";
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
    color: #1a1a2e;
    font-size: 1.8rem;
    margin-bottom: 25px;
    padding-right: 15px;
    border-right: 5px solid #4a4a6a;
    display: flex;
    align-items: center;
    gap: 10px;
}

.section-title span {
    background: #4a4a6a;
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
    background: #f0f0fa;
    border-color: #4a4a6a;
    transform: translateX(-5px);
}

.resource-icon {
    font-size: 1.5rem;
    margin-left: 12px;
    color: #4a4a6a;
}

.resource-link {
    color: #1a1a2e;
    text-decoration: none;
    font-size: 0.95rem;
    line-height: 1.6;
    flex: 1;
}

.resource-link:hover {
    color: #4a4a6a;
}

.resource-tag {
    background: #e6e6fa;
    color: #1a1a2e;
    padding: 3px 10px;
    border-radius: 20px;
    font-size: 0.75rem;
    margin-right: 10px;
    white-space: nowrap;
}

/* بخش‌های ویژه */
.special-section {
    background: linear-gradient(135deg, #f5f5fa 0%, #eaeaf5 100%);
    border-radius: 20px;
    padding: 30px;
    margin: 40px 0;
    border: 1px dashed #4a4a6a;
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
    border: 1px solid #c2c2d6;
}

.category-title {
    color: #1a1a2e;
    font-size: 1.2rem;
    font-weight: bold;
    margin-bottom: 10px;
    display: flex;
    align-items: center;
    gap: 8px;
}

.category-items {
    color: #4a4a6a;
    font-size: 0.9rem;
    line-height: 1.8;
}

/* دکمه بازگشت */
.back-button {
    display: inline-block;
    margin-top: 30px;
    padding: 12px 30px;
    background: #1a1a2e;
    color: white;
    text-decoration: none;
    border-radius: 30px;
    transition: all 0.2s;
    border: 2px solid transparent;
}

.back-button:hover {
    background: white;
    color: #1a1a2e;
    border-color: #1a1a2e;
}

/* شمارنده منابع */
.stats-bar {
    display: flex;
    gap: 15px;
    margin-bottom: 30px;
    flex-wrap: wrap;
}

.stat-item {
    background: #e6e6fa;
    padding: 8px 20px;
    border-radius: 30px;
    color: #1a1a2e;
    font-size: 0.9rem;
    display: flex;
    align-items: center;
    gap: 5px;
}

/* کارت تعاملی ویژه */
.interactive-card {
    background: linear-gradient(135deg, #2c2c44 0%, #1a1a2e 100%);
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

/* کارت کمیک */
.comic-card {
    background: linear-gradient(135deg, #ffd700 0%, #ffb347 100%);
    color: #1a1a2e;
    padding: 20px;
    border-radius: 16px;
    text-align: center;
}

.comic-card a {
    color: #1a1a2e;
    font-weight: bold;
    text-decoration: none;
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
    <div class="chapter-title">🌑 فصل پنجم: ماده تاریک</div>
    <div class="chapter-subtitle">جرم گمشده | عدسی گرانشی | ذرات فرضی | ۸۵٪ جهان</div>
    <div style="display: flex; gap: 15px; margin-top: 20px; flex-wrap: wrap;">
        <span style="background: rgba(255,255,255,0.2); padding: 5px 15px; border-radius: 30px;">📺 ۱۰ ویدیو</span>
        <span style="background: rgba(255,255,255,0.2); padding: 5px 15px; border-radius: 30px;">🎮 ۵ تعاملی</span>
        <span style="background: rgba(255,255,255,0.2); padding: 5px 15px; border-radius: 30px;">🌐 ۷ وبسایت</span>
        <span style="background: rgba(255,255,255,0.2); padding: 5px 15px; border-radius: 30px;">🎬 ۵ مستند</span>
    </div>
</div>

<!-- آمار سریع -->
<div class="stats-bar">
    <span class="stat-item">📊 مجموع منابع: ۳۰ منبع</span>
    <span class="stat-item">⏱ مناسب برای: ۷ ساعت آموزش</span>
    <span class="stat-item">🎯 سطح: متوسط تا پیشرفته</span>
    <span class="stat-item">🌑 کشف: ۱۹۳۳ - فریتز زوئیکی</span>
</div>

<!-- 📺 ویدیوها -->
<div class="content-section">
    <div class="section-title">
        📺 ویدیوهای آموزشی <span>۱۰ منبع</span>
    </div>
    <div class="resources-grid">
        <!-- مفاهیم پایه -->
        <div class="resource-item">
            <span class="resource-icon">🌑</span>
            <a href="https://www.ted.com/talks/patricia_burchat_shedding_light_on_dark_matter/transcript?language=en" class="resource-link" target="_blank">
                <strong>پرتوافکنی بر ماده تاریک</strong>
                <span class="resource-tag">TED</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">🔍</span>
            <a href="https://www.youtube.com/watch?v=6etTERFUlUI" class="resource-link" target="_blank">
                <strong>جستجوی پوچ برای ماده تاریک</strong>
                <span class="resource-tag">پیشرفته</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">🎓</span>
            <a href="https://www.youtube.com/watch?v=97NtbrTfP3Y" class="resource-link" target="_blank">
                <strong>ماده تاریک چیست؟ یک اخترفیزیک‌دان توضیح می‌دهد</strong>
                <span class="resource-tag">پایه</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">📚</span>
            <a href="https://www.youtube.com/watch?v=9W3RsaWuCuE" class="resource-link" target="_blank">
                <strong>ماده تاریک: دوره فشرده نجوم</strong>
                <span class="resource-tag">پایه</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">👤</span>
            <a href="https://www.youtube.com/watch?v=8-t-1EkOhAE" class="resource-link" target="_blank">
                <strong>راهنمای مبتدیان برای ماده تاریک</strong>
                <span class="resource-tag">پایه</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">🎙️</span>
            <a href="https://www.youtube.com/watch?v=HneiEA1B8ks" class="resource-link" target="_blank">
                <strong>ماده تاریک: ماده‌ای که نمی‌توانیم ببینیم - جیمز گیلیس</strong>
                <span class="resource-tag">پایه</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">⚛️</span>
            <a href="https://www.youtube.com/watch?v=fidzLZQyaJE" class="resource-link" target="_blank">
                <strong>آیا ماده تاریک از ذرات تشکیل شده است؟</strong>
                <span class="resource-tag">پیشرفته</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">🎯</span>
            <a href="https://www.ted.com/talks/risa_wechsler_the_search_for_dark_matter_and_what_we_ve_found_so_far/transcript?language=en&subtitle=en" class="resource-link" target="_blank">
                <strong>جستجو برای ماده تاریک - و آنچه تاکنون یافته‌ایم</strong>
                <span class="resource-tag">TED</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">⭐</span>
            <a href="https://www.youtube.com/watch?v=uBbxXNhZ78c" class="resource-link" target="_blank">
                <strong>نیل دگراس تایسون: ماده تاریک چیست؟</strong>
                <span class="resource-tag">پایه</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">🌀</span>
            <a href="https://www.youtube.com/watch?v=5LW_2J2qs0Y" class="resource-link" target="_blank">
                <strong>سوی تاریک جهان - برایان گرین</strong>
                <span class="resource-tag">پیشرفته</span>
            </a>
        </div>
    </div>
</div>

<!-- 🎮 تعاملی و اینفوگرافیک‌ها -->
<div class="content-section">
    <div class="section-title">
        🎮 تعاملی و اینفوگرافیک‌ها <span>۵ منبع</span>
    </div>
    <div class="interactive-card">
        <div style="font-size: 2.5rem; margin-bottom: 10px;">🌀</div>
        <a href="https://demonstrations.wolfram.com/GravitationalLensingByAPointMass/" target="_blank">
            🌌 عدسی‌گرانشی توسط یک جرم نقطه‌ای
        </a>
        <p style="margin-top: 15px; color: rgba(255,255,255,0.9);">
            شبیه‌ساز تعاملی خمیدگی نور در میدان گرانشی
        </p>
    </div>
    
    <div class="resources-grid" style="margin-top: 20px;">
        <div class="resource-item">
            <span class="resource-icon">🔭</span>
            <a href="https://www.jpl.nasa.gov/edu/teach/activity/how-do-we-see-dark-matter/" class="resource-link" target="_blank">
                <strong>چگونه ماده تاریک را می‌بینیم؟</strong>
                <span class="resource-tag">ناسا</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">📊</span>
            <a href="https://www.interactions.org/sites/default/files/dark-matter-infographic-STFC-UK.png" class="resource-link" target="_blank">
                <strong>اینفوگرافیک ماده تاریک</strong>
                <span class="resource-tag">تصویری</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">😄</span>
            <a href="https://phdcomics.com/comics/archive.php?comicid=1430" class="resource-link" target="_blank">
                <strong>کمیک دکتری درباره ماده تاریک</strong>
                <span class="resource-tag">طنز علمی</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">🍬</span>
            <a href="https://www.youtube.com/watch?v=UDfG69K5t6k" class="resource-link" target="_blank">
                <strong>جهان آبنبات ژله‌ای (ماده تاریک)</strong>
                <span class="resource-tag">انیمیشن</span>
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
            <span class="resource-icon">🌍</span>
            <a href="https://taraenergy.com/blog/dark-energy-and-dark-matter-explained/" class="resource-link" target="_blank">
                <strong>ماده تاریک: کاوش در منشأ جهان</strong>
                <span class="resource-tag">آموزشی</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">🔬</span>
            <a href="https://scitechdaily.com/science-made-simple-what-is-dark-matter/?utm_content=cmp-true" class="resource-link" target="_blank">
                <strong>علم ساده‌شده: ماده تاریک چیست؟</strong>
                <span class="resource-tag">SciTech</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">🚀</span>
            <a href="https://science.nasa.gov/astrophysics/focus-areas/what-is-dark-energy/" class="resource-link" target="_blank">
                <strong>ماده تاریک: ناسا</strong>
                <span class="resource-tag">ناسا</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">📰</span>
            <a href="https://www.space.com/20930-dark-matter.html" class="resource-link" target="_blank">
                <strong>ماده تاریک چیست؟: Space.com</strong>
                <span class="resource-tag">Space</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">⚛️</span>
            <a href="https://home.cern/science/physics/dark-matter" class="resource-link" target="_blank">
                <strong>ماده تاریک - سرن</strong>
                <span class="resource-tag">CERN</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">📘</span>
            <a href="https://www.interactions.org/dark-matter-day/educational-resources" class="resource-link" target="_blank">
                <strong>فیزیک قرن ۲۱ آنا‌برگ لرنر: ماده تاریک</strong>
                <span class="resource-tag">آموزشی</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">🌀</span>
            <a href="https://universe.nasa.gov/news/290/how-gravity-warps-light/" class="resource-link" target="_blank">
                <strong>گرانش چگونه نور را خم می‌کند؟</strong>
                <span class="resource-tag">ناسا</span>
            </a>
        </div>
    </div>
</div>

<!-- 🎬 مستندها -->
<div class="content-section">
    <div class="section-title">
        🎬 مستندهای علمی <span>۵ منبع</span>
    </div>
    <div class="resources-grid">
        <div class="resource-item">
            <span class="resource-icon">🎞️</span>
            <a href="https://www.youtube.com/watch?v=eBGHUn1yXeM" class="resource-link" target="_blank">
                <strong>اسرار ماده تاریک - مستند فضایی</strong>
                <span class="resource-tag">مستند</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">🕳️</span>
            <a href="https://www.youtube.com/watch?v=CM_VPjSCG8I" class="resource-link" target="_blank">
                <strong>سوی تاریک - سیاه‌چاله‌ها و ماده نامرئی</strong>
                <span class="resource-tag">مستند</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">❓</span>
            <a href="https://www.youtube.com/watch?v=fX_1pM64uUk" class="resource-link" target="_blank">
                <strong>ماده تاریک و انرژی تاریک از کجا آمدند؟</strong>
                <span class="resource-tag">مستند</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">📺</span>
            <a href="https://www.dailymotion.com/video/x226e38" class="resource-link" target="_blank">
                <strong>بی‌بی‌سی - هورایزن - ۲۰۰۶ - بیشتر جهان ما گمشده است</strong>
                <span class="resource-tag">BBC</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">🦈</span>
            <a href="https://www.youtube.com/watch?v=CM_VPjSCG8I" class="resource-link" target="_blank">
                <strong>سوی تاریک جهان - کانال دیسکاوری</strong>
                <span class="resource-tag">Discovery</span>
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
            <a href="https://quizizz.com/admin/quiz/5cb761ef3542f8001a8e753b/dark-matter" class="resource-link" target="_blank">
                <strong>ماده تاریک</strong>
                <span class="resource-tag">Quizizz</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">🌐</span>
            <a href="https://imagine.gsfc.nasa.gov/science/activities/quiz_l1/dark_matter_quiz.html" class="resource-link" target="_blank">
                <strong>آزمون ماده تاریک</strong>
                <span class="resource-tag">ناسا</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">❓</span>
            <a href="https://www.funtrivia.com/trivia-quiz/SciTech/The-Mystery-of-Dark-Matter-and-Dark-Energy-366588.html" class="resource-link" target="_blank">
                <strong>راز ماده تاریک و انرژی تاریک</strong>
                <span class="resource-tag">FunTrivia</span>
            </a>
        </div>
    </div>
</div>

<!-- دسته‌بندی موضوعی -->
<div class="special-section">
    <div style="display: flex; align-items: center; gap: 10px; margin-bottom: 20px;">
        <span style="font-size: 2rem;">📊</span>
        <h2 style="color: #1a1a2e; margin: 0;">دسته‌بندی موضوعی منابع</h2>
    </div>
    
    <div class="topic-categories">
        <div class="category-card">
            <div class="category-title">
                <span>📘</span> مفاهیم پایه
            </div>
            <div class="category-items">
                ویدیوهای ۳، ۴، ۵، ۶، ۹<br>
                مناسب برای شروع
            </div>
        </div>
        
        <div class="category-card">
            <div class="category-title">
                <span>🔬</span> تحقیقات پیشرفته
            </div>
            <div class="category-items">
                ویدیوهای ۱، ۲، ۷، ۸<br>
                جستجوهای تجربی
            </div>
        </div>
        
        <div class="category-card">
            <div class="category-title">
                <span>🖼️</span> ابزارهای بصری
            </div>
            <div class="category-items">
                ۵ ابزار تعاملی<br>
                اینفوگرافیک و کمیک
            </div>
        </div>
        
        <div class="category-card">
            <div class="category-title">
                <span>🏛️</span> منابع معتبر
            </div>
            <div class="category-items">
                ناسا، سرن، اسپیس<br>
                ۷ وبسایت علمی
            </div>
        </div>
        
        <div class="category-card">
            <div class="category-title">
                <span>🎬</span> مستندهای جذاب
            </div>
            <div class="category-items">
                ۵ مستند از BBC، دیسکاوری<br>
                کاوش در اسرار ماده تاریک
            </div>
        </div>
    </div>
</div>

<!-- نقل قول -->
<div style="background: #1a1a2e; border-radius: 16px; padding: 30px; margin: 30px 0; text-align: center; border: 1px solid #4a4a6a;">
    <span style="font-size: 2.5rem; color: white;">🌑</span>
    <p style="font-size: 1.3rem; color: white; font-style: italic; margin: 15px 0;">
        "ما از پنج درصد جهان می‌فهمیم و به آن ماده معمولی می‌گوییم. 
        نود و پنج درصد دیگر هنوز یک راز است."
    </p>
    <p style="color: #a0a0c0; font-weight: bold;">- فرانسیسکا زولو، اخترفیزیک‌دان</p>
</div>

<!-- نکات استفاده -->
<div style="background: #f5f5fa; border-radius: 16px; padding: 25px; margin-top: 30px; border-right: 5px solid #4a4a6a;">
    <h3 style="color: #1a1a2e; display: flex; align-items: center; gap: 10px;">
        <span>💡</span> نکات استفاده
    </h3>
    <ul style="color: #1a1a2e; line-height: 1.8; padding-right: 20px;">
        <li>منابع به تفکیک مفاهیم پایه و تحقیقات پیشرفته دسته‌بندی شده‌اند</li>
        <li>مناسب برای آموزش یکی از بزرگترین اسرار کیهانشناسی مدرن</li>
        <li>شبیه‌ساز عدسی گرانشی را حتماً تجربه کنید - درک بصری عالی از ماده تاریک می‌دهد</li>
        <li>کمیک دکتری نگاه طنزآمیزی به چالش‌های تحقیق دارد</li>
        <li>مستند BBC "بیشتر جهان ما گمشده است" یک کلاسیک است</li>
    </ul>
</div>

<!-- دکمه بازگشت -->
<div style="text-align: center; margin-top: 40px;">
    <a href="/books/cosmoverse/cosmic_library/main_cosmic_library" class="back-button">
        ← بازگشت به کتابخانه کیهانی
    </a>
</div>

</div>