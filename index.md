---
title: گروه هُماپران دانش
layout: page
show_sidebar: false
hero_image: img/cmb.jpg
---

<style>
  .hero-section {
    text-align: center;
    padding: 4rem 1rem;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    color: white;
    border-radius: 10px;
    margin-bottom: 3rem;
  }
  
  .logo-text {
    font-size: 3rem;
    font-weight: bold;
    text-shadow: 2px 2px 4px rgba(0,0,0,0.2);
  }
  
  .tagline {
    font-size: 1.5rem;
    margin: 1rem 0 2rem;
    opacity: 0.95;
  }
  
  .cta-button {
    background: white;
    color: #667eea;
    padding: 1rem 2.5rem;
    border-radius: 50px;
    font-size: 1.2rem;
    font-weight: bold;
    text-decoration: none;
    transition: transform 0.3s, box-shadow 0.3s;
    display: inline-block;
  }
  
  .cta-button:hover {
    transform: translateY(-3px);
    box-shadow: 0 10px 20px rgba(0,0,0,0.1);
  }
  
  .features {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 2rem;
    margin: 4rem 0;
  }
  
  .feature-card {
    text-align: center;
    padding: 2rem;
    background: #f8f9fa;
    border-radius: 10px;
    transition: all 0.3s;
  }
  
  .feature-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 5px 20px rgba(0,0,0,0.1);
  }
  
  .feature-icon {
    font-size: 2.5rem;
    margin-bottom: 1rem;
  }
  
  .book-highlight {
    background: linear-gradient(145deg, #ffffff, #f5f5f5);
    padding: 3rem;
    border-radius: 20px;
    margin: 3rem 0;
    border: 1px solid #eaeaea;
    display: flex;
    align-items: center;
    gap: 2rem;
    flex-wrap: wrap;
  }
  
  .book-info {
    flex: 1;
    min-width: 250px;
  }
  
  .book-badge {
    background: #ff6b6b;
    color: white;
    padding: 0.5rem 1rem;
    border-radius: 50px;
    display: inline-block;
    font-size: 0.9rem;
    margin-bottom: 1rem;
  }
  
  .member-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 2rem;
    margin-top: 2rem;
  }
  
  .member-card {
    position: relative;
    border-radius: 10px;
    overflow: hidden;
    box-shadow: 0 3px 10px rgba(0,0,0,0.1);
    transition: transform 0.3s;
  }
  
  .member-card:hover {
    transform: translateY(-5px);
  }
  
  .member-card img {
    width: 100%;
    height: 200px;
    object-fit: cover;
  }
  
  .member-info {
    padding: 1rem;
    background: white;
    text-align: center;
  }
  
  .nav-tabs {
    display: flex;
    justify-content: center;
    gap: 1rem;
    margin: 2rem 0;
  }
  
  .nav-tab {
    padding: 0.75rem 1.5rem;
    background: #f1f3f5;
    border-radius: 8px;
    text-decoration: none;
    color: #495057;
    font-weight: 500;
    transition: all 0.3s;
  }
  
  .nav-tab:hover, .nav-tab.active {
    background: #667eea;
    color: white;
  }
</style>

<!-- صفحه اصلی - لندینگ پیج -->
<div class="hero-section">
  <div class="logo-text">هُماپران دانش</div>
  <div class="tagline">گسترش دانش عمومی و تخصصی در فیزیک و کیهان‌شناسی</div>
  <a href="/activities" class="cta-button">✨ مشاهده فعالیت‌ها</a>
</div>

<!-- منوی تب‌ها -->
<div class="nav-tabs">
  <a href="/" class="nav-tab active">🏠 صفحه اصلی</a>
  <a href="/activities" class="nav-tab">📋 فعالیت‌ها</a>
  <a href="/books/main_books" class="nav-tab">📚 کتاب‌ها</a>
  <a href="/team" class="nav-tab">👥 اعضا</a>
</div>

<!-- ویژگی‌های کلیدی -->
<div class="features">
  <div class="feature-card">
    <div class="feature-icon">🎙️</div>
    <h3>محتوای چندرسانه‌ای</h3>
    <p>پادکست‌ها و اپیزودهای علمی-آموزشی</p>
  </div>
  
  <div class="feature-card">
    <div class="feature-icon">📖</div>
    <h3>ترجمه و بومی‌سازی</h3>
    <p>کتاب‌های علمی تخصصی برای مخاطب فارسی</p>
  </div>
  
  <div class="feature-card">
    <div class="feature-icon">🎓</div>
    <h3>آموزش نوین</h3>
    <p>حضوری و آنلاین با رویکردی جدید</p>
  </div>
</div>

<!-- دستاورد ویژه -->
<div class="book-highlight">
  <div class="book-info">
    <span class="book-badge">🎉 اولین دستاورد</span>
    <h2 style="margin: 1rem 0; font-size: 1.8rem;">ماجراهای کیهان</h2>
    <p style="font-size: 1.1rem; line-height: 1.6; color: #4a5568;">
      به همکاری با <strong>انتشارات مبتکران</strong>، نخستین اثر گروه هُماپران دانش منتشر شد.
    </p>
    <a href="/books/cosmoverse" style="display: inline-block; margin-top: 1rem; color: #667eea; font-weight: bold; text-decoration: none;">
      بیشتر بدانید ←
    </a>
  </div>
  <div style="flex: 0 0 100px; text-align: center;">
    <div style="font-size: 5rem;">📚</div>
  </div>
</div>


<!-- برای اعضای گروه -->
<style>
  .member-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
    gap: 2.5rem;
    margin-top: 2rem;
  }
  
  .member-card {
    text-align: center;
    padding: 1.5rem 4.5rem;
    background: white;
    border-radius: 50px;
    box-shadow: 0 5px 20px rgba(0,0,0,0.03);
    transition: transform 0.3s, box-shadow 0.3s;
    border: 1px solid #f0f0f0;
  }
  
  .member-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 15px 30px rgba(102, 126, 234, 0.1);
    border-color: #667eea;
  }
  
  /* عکس گرد با حاشیه */
  .member-image {
    width: 150px;
    height: 150px;
    border-radius: 50%;
    object-fit: cover;
    border: 4px solid white;
    box-shadow: 0 8px 20px rgba(0,0,0,0.1);
    margin-bottom: 1rem;
    transition: border-color 0.3s;
  }
  
  .member-card:hover .member-image {
    border-color: #667eea;
  }
  
  .member-name {
    font-size: 1.2rem;
    font-weight: bold;
    margin: 0.5rem 0 0.2rem;
    color: #2d3748;
  }
  
  .member-role {
    color: #718096;
    font-size: 0.9rem;
    margin-bottom: 1rem;
    padding-bottom: 1rem;
    border-bottom: 1px dashed #e2e8f0;
  }
  
  /* ایمیل با آیکون */
  .member-email {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    gap: 0.5rem;
    color: #4a5568;
    text-decoration: none;
    font-size: 0.4rem;
    padding: 0.5rem 1rem;
    background: #f7fafc;
    border-radius: 10px;
    transition: all 0.3s;
    border: 1px solid #e2e8f0;
    width: 100%;
    box-sizing: border-box;
  }
  
  .member-email:hover {
    background: #667eea;
    color: white;
    border-color: #667eea;
  }
  
  .member-email:hover .email-icon {
    color: white;
  }
  
  .email-icon {
    font-size: 1.1rem;
    color: #667eea;
  }
  
  /* یا استفاده از آیکون شبه‌عنصر */
  .member-email::before {
    content: "✉️";
    font-size: 1.1rem;
  }
  
  /* نسخه فونت‌آسوم (اگه دارید) */
  .fas.fa-envelope {
    margin-right: 0.3rem;
  }
</style>

<!-- بخش اعضای گروه با طراحی جدید -->
<div style="text-align: center; margin: 3rem 0 1rem;">
  <h2 style="font-size: 2rem; margin-bottom: 0.5rem; color: #2d3748;">👥 اعضای گروه</h2>
  <p style="color: #718096; margin-bottom: 2rem; font-size: 1.1rem;">
    تیم علمی هُماپران دانش
  </p>
</div>

<div class="member-grid">
  <!-- ریحانه کریمی -->
  <div class="member-card">
    <img src="img/rei.png" alt="ریحانه کریمی" class="member-image">
    <h3 class="member-name">ریحانه کریمی</h3>
    <div class="member-role">محقق و مدرس فیزیک</div>
    <a href="mailto:reihanehkariimii@gmail.com" class="member-email">
      reihanehkariimii@gmail.com
    </a>
  </div>
  
  <!-- سحر محمدی -->
  <div class="member-card">
    <img src="img/sahar.png" alt="سحر محمدی" class="member-image">
    <h3 class="member-name">سحر محمدی</h3>
    <div class="member-role">محقق کیهان‌شناسی</div>
    <a href="mailto:sahar.mohammadi7799@gmail.com" class="member-email">
      sahar.mohammadi7799@gmail.com
    </a>
  </div>
  
  <!-- ابراهیم یوسفی -->
  <div class="member-card">
    <img src="img/ebrahim.png" alt="ابراهیم یوسفی" class="member-image">
    <h3 class="member-name">ابراهیم یوسفی</h3>
    <div class="member-role">مدرس و مترجم</div>
    <a href="mailto:eyph2009@gmail.com" class="member-email">
      eyph2009@gmail.com
    </a>
  </div>
  
  <!-- علیرضا طالبیان -->
  <div class="member-card">
    <img src="img/alireza.png" alt="علیرضا طالبیان" class="member-image">
    <h3 class="member-name">علیرضا طالبیان</h3>
    <div class="member-role">پژوهشگر پسادکتری</div>
    <a href="mailto:talebian@ipm.ir" class="member-email">
      talebian@ipm.ir
    </a>
  </div>
</div>



<div style="text-align: center; margin: 3rem 0;">
  <a href="/team" style="color: #667eea; text-decoration: none; font-weight: bold;">مشاهده همه اعضا ←</a>
</div>