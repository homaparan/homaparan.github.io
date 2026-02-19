---
layout: page
title: کتابخانه کیهانی - فصل چهارم
subtitle: گرانش هندسی | نسبیت عام | فضا-زمان
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
    background: linear-gradient(135deg, #1a2e4f 0%, #2c3e6e 100%);
    color: white;
    padding: 40px;
    border-radius: 30px;
    margin-bottom: 40px;
    position: relative;
    overflow: hidden;
    box-shadow: 0 15px 30px rgba(44, 62, 110, 0.4);
}

.chapter-header::before {
    content: "🌀";
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
    color: #1a3c6e;
    font-size: 1.8rem;
    margin-bottom: 25px;
    padding-right: 15px;
    border-right: 5px solid #4a6fa5;
    display: flex;
    align-items: center;
    gap: 10px;
}

.section-title span {
    background: #4a6fa5;
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
    border-color: #4a6fa5;
    transform: translateX(-5px);
}

.resource-icon {
    font-size: 1.5rem;
    margin-left: 12px;
    color: #4a6fa5;
}

.resource-link {
    color: #1a3c6e;
    text-decoration: none;
    font-size: 0.95rem;
    line-height: 1.6;
    flex: 1;
}

.resource-link:hover {
    color: #4a6fa5;
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
    background: linear-gradient(135deg, #f0f4fa 0%, #e6edf7 100%);
    border-radius: 20px;
    padding: 30px;
    margin: 30px 0;
    border: 2px solid #4a6fa5;
    position: relative;
    overflow: hidden;
}

.featured-video::before {
    content: "🎳";
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
    border-right: 3px solid #4a6fa5;
}

.featured-link {
    display: inline-flex;
    align-items: center;
    gap: 10px;
    background: #4a6fa5;
    color: white;
    padding: 12px 25px;
    border-radius: 30px;
    text-decoration: none;
    font-weight: bold;
    margin-top: 15px;
    transition: all 0.2s;
}

.featured-link:hover {
    background: #2c3e6e;
    transform: scale(1.05);
}

/* بخش‌های ویژه */
.special-section {
    background: linear-gradient(135deg, #f0f4fa 0%, #e6edf7 100%);
    border-radius: 20px;
    padding: 30px;
    margin: 40px 0;
    border: 1px dashed #4a6fa5;
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

/* کارت تعاملی ویژه */
.interactive-card {
    background: linear-gradient(135deg, #4a6fa5 0%, #2c5aa0 100%);
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

/* دکمه بازگشت */
.back-button {
    display: inline-block;
    margin-top: 30px;
    padding: 12px 30px;
    background: #4a6fa5;
    color: white;
    text-decoration: none;
    border-radius: 30px;
    transition: all 0.2s;
    border: 2px solid transparent;
}

.back-button:hover {
    background: white;
    color: #4a6fa5;
    border-color: #4a6fa5;
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
    <div class="chapter-title">🌀 فصل چهارم: گرانش هندسی</div>
    <div class="chapter-subtitle">نسبیت عام | نسبیت خاص | فضا-زمان | خمیدگی فضا</div>
    <div style="display: flex; gap: 15px; margin-top: 20px; flex-wrap: wrap;">
        <span style="background: rgba(255,255,255,0.2); padding: 5px 15px; border-radius: 30px;">📺 ۱۱ ویدیو</span>
        <span style="background: rgba(255,255,255,0.2); padding: 5px 15px; border-radius: 30px;">🎮 ۶ تعاملی</span>
        <span style="background: rgba(255,255,255,0.2); padding: 5px 15px; border-radius: 30px;">🌐 ۳ وبسایت</span>
        <span style="background: rgba(255,255,255,0.2); padding: 5px 15px; border-radius: 30px;">🎬 ۴ مستند</span>
    </div>
</div>

<!-- آمار سریع -->
<div class="stats-bar">
    <span class="stat-item">📊 مجموع منابع: ۲۷ منبع</span>
    <span class="stat-item">⏱ مناسب برای: ۸ ساعت آموزش</span>
    <span class="stat-item">🎯 سطح: پیشرفته</span>
    <span class="stat-item">🧠 کشف: ۱۹۱۵ - آلبرت اینشتین</span>
</div>

<!-- ویدیوی ویژه: آزمایش اتاق خلأ -->
<div class="featured-video">
    <div class="featured-title">
        <span>🎳</span> ویدیوی ویژه کلاس درس: آزمایش سقوط آزاد
    </div>
    
    <div style="display: flex; align-items: center; gap: 20px; flex-wrap: wrap;">
        <div style="flex: 1; min-width: 250px;">
            <img src="../../img/gravity-vacuum-chamber.jpg" alt="آزمایش اتاق خلأ - توپ بولینگ و پر" style="width: 100%; max-width: 300px; border-radius: 16px; box-shadow: 0 8px 20px rgba(0,0,0,0.1);" onerror="this.style.display='none'">
        </div>
        <div style="flex: 2;">
            <div class="featured-description">
                <strong>🎓 گفتگوی کلاسی:</strong>
                <p style="margin-top: 10px;">
                    <span style="background: #4a6fa5; color: white; padding: 3px 10px; border-radius: 20px; font-size: 0.8rem;">دبیر</span>
                    <br>
                    "عالی است، درست گفتید! امروز می‌خواهیم درباره گرانش صحبت کنیم. اما قبل از آن، بیایید این ویدیو را تماشا کنیم."
                </p>
                <p style="margin-top: 10px; font-style: italic; color: #6c757d;">
                    (معلم ویدیویی از یک توپ بولینگ و یک پر بزرگ در حال سقوط در اتاق خلأ پخش می‌کند.)
                </p>
                <p style="margin-top: 10px;">
                    <span style="background: #4a6fa5; color: white; padding: 3px 10px; border-radius: 20px; font-size: 0.8rem;">دبیر</span>
                    <br>
                    "قبل از شروع، کدام‌یک از شما می‌تواند پیش‌بینی کند که زودتر سقوط می‌کند؟"
                </p>
                <p style="margin-top: 10px;">
                    <span style="background: #ffc107; color: #1a3c6e; padding: 3px 10px; border-radius: 20px; font-size: 0.8rem;">لئو</span>
                    <br>
                    "منطقی است که توپ بولینگ زودتر سقوط کند چون سنگین‌تر است."
                </p>
                <p style="margin-top: 10px;">
                    <span style="background: #4a6fa5; color: white; padding: 3px 10px; border-radius: 20px; font-size: 0.8rem;">دبیر</span>
                    <br>
                    "بیایید تماشا کنیم و مشاهده کنیم."
                </p>
                <p style="margin-top: 10px;">
                    <span style="background: #ffc107; color: #1a3c6e; padding: 3px 10px; border-radius: 20px; font-size: 0.8rem;">لئو</span>
                    <br>
                    "وای! هر دو دقیقاً هم‌زمان سقوط کردند!"
                </p>
            </div>
            
            <div class="featured-quote">
                <p>📺 این بخش از مستند "Human Universe" محصول BBC گرفته شده است.</p>
            </div>
            
            <a href="https://www.youtube.com/watch?v=frZ9dN_ATew" class="featured-link" target="_blank">
                🎬 تماشای ویدیوی آزمایش سقوط آزاد (اتاق خلأ)
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
        <!-- نسبیت عام -->
        <div class="resource-item">
            <span class="resource-icon">🌀</span>
            <a href="https://www.youtube.com/watch?v=XRr1kaXKBsU" class="resource-link" target="_blank">
                <strong>چرا گرانش یک نیرو نیست؟</strong>
                <span class="resource-tag">نسبیت عام</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">📐</span>
            <a href="https://www.youtube.com/watch?v=XRr1kaXKBsU" class="resource-link" target="_blank">
                <strong>نسبیت عام به سادگی و بصری توضیح داده شده</strong>
                <span class="resource-tag">نسبیت عام</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">💡</span>
            <a href="https://www.youtube.com/watch?v=tzQC3uYL67U" class="resource-link" target="_blank">
                <strong>اگر نور جرم ندارد، چرا تحت تأثیر گرانش قرار می‌گیرد؟</strong>
                <span class="resource-tag">نسبیت عام</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">📚</span>
            <a href="https://www.youtube.com/watch?v=KXhJDPu0G-E" class="resource-link" target="_blank">
                <strong>نظریه نسبیت عام</strong>
                <span class="resource-tag">نسبیت عام</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">🎤</span>
            <a href="https://www.youtube.com/watch?v=0jjFjC30-4A" class="resource-link" target="_blank">
                <strong>برایان گرین نسبیت عام را توضیح می‌دهد</strong>
                <span class="resource-tag">نسبیت عام</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">⚡</span>
            <a href="https://www.youtube.com/watch?v=OHdV9aO6jaE" class="resource-link" target="_blank">
                <strong>گرانش چگونه بر نور تأثیر می‌گذارد؟</strong>
                <span class="resource-tag">نسبیت عام</span>
            </a>
        </div>
        
        <!-- نسبیت خاص -->
        <div class="resource-item">
            <span class="resource-icon">⏱️</span>
            <a href="https://www.youtube.com/watch?v=5BBHEZFearI" class="resource-link" target="_blank">
                <strong>نظریه نسبیت خاص اینشتین - آیا زمان واقعاً کند می‌شود؟</strong>
                <span class="resource-tag">نسبیت خاص</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">💫</span>
            <a href="https://www.youtube.com/watch?v=FyGz5WjIcCI" class="resource-link" target="_blank">
                <strong>مبانی نظریه نسبیت خاص - چرا سرعت نور ثابت است</strong>
                <span class="resource-tag">نسبیت خاص</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">🎓</span>
            <a href="https://www.youtube.com/watch?v=AInCqm5nCzw" class="resource-link" target="_blank">
                <strong>نسبیت خاص: دوره فشرده فیزیک #۴۲</strong>
                <span class="resource-tag">نسبیت خاص</span>
            </a>
        </div>
        
        <!-- آزمایش‌های بصری -->
        <div class="resource-item">
            <span class="resource-icon">🔬</span>
            <a href="https://www.youtube.com/watch?v=E43-CfukEgs" class="resource-link" target="_blank">
                <strong>برایان کاکس از بزرگترین خلأ جهان بازدید می‌کند</strong>
                <span class="resource-tag">آزمایش</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">🎨</span>
            <a href="https://www.youtube.com/watch?v=MTY1Kje0yLg&t=240s" class="resource-link" target="_blank">
                <strong>گرانش به صورت بصری</strong>
                <span class="resource-tag">تصویری</span>
            </a>
        </div>
    </div>
</div>

<!-- 🎮 ابزارهای تعاملی -->
<div class="content-section">
    <div class="section-title">
        🎮 ابزارهای تعاملی <span>۶ منبع</span>
    </div>
    <div class="interactive-card">
        <div style="font-size: 2.5rem; margin-bottom: 10px;">🪐</div>
        <a href="https://vis.sciencemag.org/generalrelativity/" target="_blank">
            🌌 نسبیت عام به گونه‌ای که هرگز ندیده‌اید
        </a>
        <p style="margin-top: 15px; color: rgba(255,255,255,0.9);">
            شبیه‌ساز تعاملی خمیدگی فضا-زمان
        </p>
    </div>
    <div class="resources-grid" style="margin-top: 20px;">
        <div class="resource-item">
            <span class="resource-icon">🪐</span>
            <a href="https://www.jpl.nasa.gov/edu/teach/activity/modeling-the-orbits-of-planets/" class="resource-link" target="_blank">
                <strong>مدل‌سازی مدارهای سیارات</strong>
                <span class="resource-tag">ناسا</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">📄</span>
            <a href="https://www.spacetimetravel.org/sectormodels2/sectormodels2_en_w.pdf" class="resource-link" target="_blank">
                <strong>جعبه ابزار آموزش نسبیت عام: II. ژئودزیک‌ها</strong>
                <span class="resource-tag">PDF</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">🕰️</span>
            <a href="https://www.edumedia-sciences.com/en/media/969-space-time-concept" class="resource-link" target="_blank">
                <strong>مفهوم فضا-زمان</strong>
                <span class="resource-tag">انیمیشن</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">⚛️</span>
            <a href="https://www.refsmmat.com/jsphys/relativity/relativity.html" class="resource-link" target="_blank">
                <strong>شبیه‌ساز نسبیت</strong>
                <span class="resource-tag">جاوا</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">⏳</span>
            <a href="https://javalab.org/en/special_relativity_en/" class="resource-link" target="_blank">
                <strong>نسبیت خاص: اتساع زمان</strong>
                <span class="resource-tag">شبیه‌ساز</span>
            </a>
        </div>
    </div>
</div>

<!-- 🌐 وبسایت‌ها و مقالات -->
<div class="content-section">
    <div class="section-title">
        🌐 وبسایت‌ها و مقالات <span>۳ منبع</span>
    </div>
    <div class="resources-grid">
        <div class="resource-item">
            <span class="resource-icon">🌍</span>
            <a href="https://www.einstein-online.info/en/category/elementary/general-relativity-elementary/" class="resource-link" target="_blank">
                <strong>اینشتین آنلاین</strong>
                <span class="resource-tag">مرجع</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">📘</span>
            <a href="https://www.viten.no/filarkiv/general-relativity/#/" class="resource-link" target="_blank">
                <strong>نسبیت عام</strong>
                <span class="resource-tag">آموزشی</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">📰</span>
            <a href="https://www.newyorker.com/tech/annals-of-technology/the-space-doctors-big-idea-einstein-general-relativity#ampshare%3Dhttp%3A%2F%2Fwww.newyorker.com%2Ftech%2Felements%2Fthe-space-doctors-big-idea-einstein-general-relativity" class="resource-link" target="_blank">
                <strong>ایده بزرگ دکتر فضایی</strong>
                <span class="resource-tag">نیویورکر</span>
            </a>
        </div>
    </div>
</div>

<!-- 🎬 مستندها -->
<div class="content-section">
    <div class="section-title">
        🎬 مستندهای علمی <span>۴ منبع</span>
    </div>
    <div class="resources-grid">
        <div class="resource-item">
            <span class="resource-icon">🧠</span>
            <a href="https://www.youtube.com/watch?v=EZtfMhjLySI" class="resource-link" target="_blank">
                <strong>درون ذهن آلبرت اینشتین</strong>
                <span class="resource-tag">مستند</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">🌀</span>
            <a href="https://www.youtube.com/watch?v=ka122yNTJ3c" class="resource-link" target="_blank">
                <strong>مستند نظریه نسبیت عام</strong>
                <span class="resource-tag">مستند</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">💡</span>
            <a href="https://www.pbslearningmedia.org/resource/nvfb-sci-einsteinsidea/wgbh-nova-einsteins-big-idea-full-length-broadcast/" class="resource-link" target="_blank">
                <strong>ایده بزرگ اینشتین، پی‌بی‌اس نوا</strong>
                <span class="resource-tag">PBS</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">🌠</span>
            <a href="https://www.youtube.com/watch?v=UgudCmLobxw" class="resource-link" target="_blank">
                <strong>جهان اینشتین: درک نظریه نسبیت عام</strong>
                <span class="resource-tag">مستند</span>
            </a>
        </div>
    </div>
</div>

<!-- ❓ آزمون‌ها و بازی‌ها -->
<div class="content-section">
    <div class="section-title">
        ❓ آزمون‌ها و بازی‌ها <span>۴ منبع</span>
    </div>
    <div class="resources-grid">
        <div class="resource-item">
            <span class="resource-icon">📝</span>
            <a href="https://study.com/academy/practice/quiz-worksheet-practice-analysis-of-the-general-theory-of-relativity.html" class="resource-link" target="_blank">
                <strong>نظریه عام نسبیت</strong>
                <span class="resource-tag">آزمون</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">📝</span>
            <a href="https://www.school-for-champions.com/science/mini-quiz_gravitation_relativity.htm" class="resource-link" target="_blank">
                <strong>نظریه گرانش نسبیت</strong>
                <span class="resource-tag">آزمون</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">🃏</span>
            <a href="https://quizlet.com/127337504/sr-general-relativity-quiz-flash-cards/" class="resource-link" target="_blank">
                <strong>کارت‌های فلش نسبیت</strong>
                <span class="resource-tag">Quizlet</span>
            </a>
        </div>
        
        <div class="resource-item">
            <span class="resource-icon">🎮</span>
            <a href="https://testtubegames.com/srel101.html" class="resource-link" target="_blank">
                <strong>نسبیت ۱۰۱</strong>
                <span class="resource-tag">بازی</span>
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
                <span>🌀</span> نسبیت عام
            </div>
            <div class="category-items">
                ویدیوهای ۱، ۲، ۳، ۴، ۶<br>
                شبیه‌ساز ScienceMag
            </div>
        </div>
        
        <div class="category-card">
            <div class="category-title">
                <span>⚡</span> نسبیت خاص
            </div>
            <div class="category-items">
                ویدیوهای ۵، ۷، ۸، ۹<br>
                شبیه‌ساز اتساع زمان
            </div>
        </div>
        
        <div class="category-card">
            <div class="category-title">
                <span>🔬</span> آزمایش‌های بصری
            </div>
            <div class="category-items">
                ویدیوهای ۱۰، ۱۱<br>
                آزمایش اتاق خلأ (Human Universe)
            </div>
        </div>
        
        <div class="category-card">
            <div class="category-title">
                <span>🛠️</span> ابزارهای تعاملی
            </div>
            <div class="category-items">
                ۶ شبیه‌ساز آموزشی<br>
                وبسایت‌های مرجع
            </div>
        </div>
        
        <div class="category-card">
            <div class="category-title">
                <span>🎬</span> مستندهای تاریخی
            </div>
            <div class="category-items">
                ۴ مستند درباره اینشتین<br>
                زندگی و کشفیات
            </div>
        </div>
    </div>
</div>

<!-- نقل قول اینشتین -->
<div style="background: #e6f0fa; border-radius: 16px; padding: 30px; margin: 30px 0; text-align: center; border: 1px solid #4a6fa5;">
    <span style="font-size: 2.5rem;">✨</span>
    <p style="font-size: 1.3rem; color: #1a3c6e; font-style: italic; margin: 15px 0;">
        "مهم این است که هرگز از پرسیدن سؤال دست نکشیم. کنجکاوی دلیل وجودی ماست."
    </p>
    <p style="color: #4a6fa5; font-weight: bold;">- آلبرت اینشتین</p>
</div>

<!-- نکات استفاده -->
<div style="background: #f0f4fa; border-radius: 16px; padding: 25px; margin-top: 30px; border-right: 5px solid #4a6fa5;">
    <h3 style="color: #1a3c6e; display: flex; align-items: center; gap: 10px;">
        <span>💡</span> نکات استفاده
    </h3>
    <ul style="color: #1a3c6e; line-height: 1.8; padding-right: 20px;">
        <li>منابع به تفکیک نسبیت عام و خاص دسته‌بندی شده‌اند</li>
        <li>مناسب برای آموزش مفاهیم پیشرفته فیزیک نظری</li>
        <li>ویدیوی آزمایش سقوط آزاد در اتاق خلأ از مستند Human Universe را حتماً ببینید</li>
        <li>شبیه‌ساز "نسبیت عام به گونه‌ای که هرگز ندیده‌اید" را حتماً تجربه کنید</li>
        <li>مستند "ایده بزرگ اینشتین" از PBS نوا، کاملترین منبع تاریخی است</li>
        <li>بازی "نسبیت ۱۰۱" برای درک شهودی اتساع زمان عالی است</li>
    </ul>
</div>

<!-- دکمه بازگشت -->
<div style="text-align: center; margin-top: 40px;">
    <a href="/books/cosmoverse/cosmic_library/main_cosmic_library" class="back-button">
        ← بازگشت به کتابخانه کیهانی
    </a>
</div>

</div>
