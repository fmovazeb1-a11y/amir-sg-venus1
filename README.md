# amir-sg-venus1
venus Research Project

<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="theme-color" content="#080d1b">
  <meta name="description" content="پروژه پژوهشی AMIR SG درباره سیاره زهره">
  <title>AMIR SG | Venus Research Project</title>

  <style>
    :root {
      --bg: #080d1b;
      --panel: #111b30;
      --text: #f4f7ff;
      --muted: #b7c5df;
      --blue: #3987ff;
      --red: #ff475d;
      --gold: #ffd27a;
    }

    * {
      box-sizing: border-box;
      scroll-behavior: smooth;
    }

    body {
      margin: 0;
      font-family: Tahoma, Arial, sans-serif;
      background:
        radial-gradient(ellipse at 15% 10%, #172f60 0, transparent 35%),
        radial-gradient(ellipse at 90% 40%, #35172e 0, transparent 30%),
        var(--bg);
      color: var(--text);
      line-height: 2;
    }

    a {
      color: inherit;
      text-decoration: none;
    }

    .topbar {
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 12px;
      padding: 16px 7%;
      border-bottom: 1px solid #ffffff18;
      background: #080d1bd9;
    }

    .brand {
      font-size: 23px;
      font-weight: bold;
      letter-spacing: 1px;
    }

    .brand span {
      color: var(--red);
    }

    .tag {
      color: var(--muted);
      font-size: 12px;
    }

    .hero {
      text-align: center;
      padding: 55px 20px 65px;
      background: linear-gradient(130deg, #173b77aa, #a62440aa);
      border-bottom: 1px solid #ffffff20;
    }

    .eyebrow {
      display: inline-block;
      padding: 4px 14px;
      border: 1px solid #ffffff45;
      border-radius: 30px;
      font-size: 13px;
      color: #e1eaff;
    }

    h1 {
      margin: 18px 0 8px;
      font-size: clamp(34px, 8vw, 62px);
      line-height: 1.4;
    }

    .hero p {
      max-width: 600px;
      margin: 10px auto 24px;
      color: #e2eaff;
    }

    .planet {
      width: 145px;
      height: 145px;
      margin: 28px auto 15px;
      display: grid;
      place-items: center;
      border-radius: 50%;
      font-size: 90px;
      background: radial-gradient(circle at 35% 30%,
        #ffe9a8, #d68b45 48%, #713b49 78%, #21182e);
      box-shadow: 0 0 45px #ffb35a55,
                  0 0 100px #d84c6b20;
      animation: float 4s ease-in-out infinite;
    }

    @keyframes float {
      0%, 100% { transform: translateY(0); }
      50% { transform: translateY(-10px); }
    }

    .button {
      display: inline-block;
      margin: 8px 4px;
      padding: 10px 22px;
      border-radius: 10px;
      background: linear-gradient(120deg, var(--blue), #6356e8);
      color: white;
      font-weight: bold;
      border: 0;
      cursor: pointer;
      font-family: inherit;
      font-size: 14px;
    }

    .button.secondary {
      background: #ffffff12;
      border: 1px solid #ffffff40;
    }

    main {
      width: min(100% - 32px, 950px);
      margin: 35px auto;
    }

    .section-title {
      font-size: 25px;
      margin: 30px 0 18px;
    }

    .section-title span {
      color: var(--gold);
    }

    .intro {
      color: var(--muted);
      text-align: justify;
    }

    .grid {
      display: grid;
      grid-template-columns: repeat(2, minmax(0, 1fr));
      gap: 16px;
    }

    .card {
      padding: 20px;
      background: linear-gradient(145deg, #15223a, #0e1729);
      border: 1px solid #ffffff17;
      border-radius: 17px;
      transition: transform .2s, border-color .2s;
    }

    .card:hover {
      transform: translateY(-4px);
      border-color: #3987ff99;
    }

    .card .emoji {
      font-size: 29px;
    }

    .card h3 {
      margin: 4px 0 8px;
      color: var(--gold);
      font-size: 18px;
    }

    .card p {
      margin: 0;
      color: var(--muted);
      font-size: 14px;
    }

    .fact {
      margin-top: 24px;
      padding: 22px;
      border-right: 4px solid var(--red);
      border-radius: 12px;
      background: #ff475d12;
    }

    .fact strong {
      color: #ff8b9a;
    }

    .stats {
      display: grid;
      grid-template-columns: repeat(3, minmax(0, 1fr));
      gap: 12px;
      margin: 25px 0;
    }

    .stat {
      padding: 15px 8px;
      text-align: center;
      background: #3987ff12;
      border: 1px solid #3987ff35;
      border-radius: 13px;
    }

    .stat strong {
      display: block;
      font-size: 21px;
      color: #8dbbff;
    }

    .stat small {
      color: var(--muted);
      font-size: 12px;
    }

    .footer {
      margin-top: 55px;
      padding: 28px 15px;
      text-align: center;
      background: #050914;
      border-top: 1px solid #ffffff17;
      color: var(--muted);
      font-size: 13px;
    }

    .footer strong {
      color: white;
    }

    @media (max-width: 580px) {
      .topbar { padding: 12px 16px; }
      .brand { font-size: 20px; }
      .tag { font-size: 10px; }
      .grid { grid-template-columns: 1fr; }
      .stats { grid-template-columns: 1fr; }
      .hero { padding-top: 40px; }
    }

    @media (prefers-reduced-motion: reduce) {
      *, *::before, *::after {
        animation: none !important;
        scroll-behavior: auto !important;
        transition: none !important;
      }
    }
  </style>
</head>

<body>
  <nav class="topbar">
    <a class="brand" href="#home">AMIR <span>SG</span></a>
    <span class="tag">SPACE RESEARCH · 2026</span>
  </nav>

  <header class="hero" id="home">
    <span class="eyebrow">پروژه پژوهشی نجوم</span>
    <div class="planet" aria-label="نماد سیاره زهره">♀</div>
    <h1>سفر به سیاره زهره</h1>
    <p>
      با یکی از شگفت‌انگیزترین سیارات منظومه شمسی آشنا شو؛
      سیاره‌ای داغ، اسرارآمیز و پوشیده از ابرهای ضخیم.
    </p>
    <a class="button" href="#research">شروع کاوش 🚀</a>
    <a class="button secondary" href="#facts">حقایق جالب</a>
  </header>

  <main id="research">
    <h2 class="section-title"><span>01.</span> زهره چیست؟</h2>
    <p class="intro">
      زهره دومین سیاره از خورشید است و از نظر اندازه شباهت زیادی
      به زمین دارد. این سیاره جو بسیار ضخیمی دارد و گرمای زیادی
      را در خود نگه می‌دارد. به همین دلیل، زهره داغ‌ترین سیاره
      منظومه شمسی است؛ حتی داغ‌تر از عطارد که به خورشید نزدیک‌تر است.
    </p>

    <div class="stats">
      <div class="stat">
        <strong>۲</strong>
        <small>جایگاه از خورشید</small>
      </div>
      <div class="stat">
        <strong>۴۶۵°C</strong>
        <small>دمای میانگین سطح</small>
      </div>
      <div class="stat">
        <strong>۲۲۵ روز</strong>
        <small>مدت یک سال زهره</small>
      </div>
    </div>

    <h2 class="section-title"><span>02.</span> ویژگی‌های شگفت‌انگیز</h2>

    <div class="grid">
      <section class="card">
        <div class="emoji">🌡️</div>
        <h3>گرمای شدید</h3>
        <p>
          دمای سطح زهره حدود ۴۶۵ درجه سانتی‌گراد است.
          اثر گلخانه‌ای شدید جو آن، گرما را به دام می‌اندازد.
        </p>
      </section>

      <section class="card">
        <div class="emoji">☁️</div>
        <h3>ابرهای اسیدی</h3>
        <p>
          جو زهره عمدتاً از دی‌اکسید کربن تشکیل شده است
          و ابرهای آن حاوی قطرات اسید سولفوریک هستند.
        </p>
      </section>

      <section class="card">
        <div class="emoji">⏳</div>
        <h3>روز طولانی</h3>
        <p>
          چرخش زهره به دور محور خودش حدود ۲۴۳ روز زمینی طول می‌کشد؛
          حتی بیشتر از مدت یک سال آن!
        </p>
      </section>

      <section class="card">
        <div class="emoji">🔄</div>
        <h3>چرخش وارونه</h3>
        <p>
          زهره برخلاف جهت چرخش بیشتر سیارات، در جهت مخالف می‌چرخد.
          بنابراین خورشید در آن از غرب طلوع می‌کند.
        </p>
      </section>
    </div>

    <section class="fact" id="facts">
      <strong>💡 آیا می‌دانستی؟</strong>
      <p>
        فشار جو در سطح زهره حدود ۹۲ برابر فشار جو زمین در سطح دریاست.
        این شرایط، کاوش مستقیم سطح آن را بسیار دشوار می‌کند.
      </p>
    </section>

    <h2 class="section-title"><span>03.</span> چرا زهره مهم است؟</h2>
    <p class="intro">
      بررسی زهره به دانشمندان کمک می‌کند اثر گلخانه‌ای، تحول جو سیارات
      و تفاوت میان زمین و جهان‌های دیگر را بهتر درک کنند.
      مأموریت‌های فضایی با استفاده از ابزارهای علمی، این سیاره را
      از راه دور بررسی می‌کنند.
    </p>

    <div style="text-align:center; margin-top:30px">
      <button class="button" onclick="window.scrollTo({top:0,behavior:'smooth'})">
        بازگشت به بالای صفحه ↑
      </button>
    </div>
  </main>

  <footer class="footer">
    <p><strong>AMIR SG</strong> | Venus Research Project</p>
    <p>یک پروژه آموزشی درباره نجوم و منظومه شمسی 🌌</p>
    <p>ساخته‌شده با ❤️ و کنجکاوی</p>
  </footer>
</body>
</html>
