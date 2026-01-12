<!doctype html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>أكاديمية عايد | دورة STEP المكثفة 2026</title>
  <meta name="description" content="دورة STEP المكثفة 2026 من أكاديمية عايد الرسمية — محتوى مركز + نماذج حديثة وتسجيل سريع وإرسال الإيصال للحساب الرسمي للتفعيل." />

  <!-- Arabic font -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Tajawal:wght@400;500;700;800;900&display=swap" rel="stylesheet">

  <!-- Tailwind CDN -->
  <script src="https://cdn.tailwindcss.com"></script>

  <style>
    :root{
      --brand-yellow:#F5C400;
      --brand-black:#0B0B0B;
      --soft-black:#111111;
    }
    html,body{font-family:"Tajawal",system-ui,-apple-system,Segoe UI,Roboto,Arial,sans-serif;background:var(--brand-black)}
    /* watermark */
    .watermark::before{
      content:"أكاديمية عايد • STEP المكثفة 2026 • Ayed Academy";
      position:fixed; inset:-200px;
      display:flex; align-items:center; justify-content:center;
      transform:rotate(-18deg);
      color:rgba(255,255,255,.05);
      font-weight:900;
      font-size:42px;
      letter-spacing:1px;
      pointer-events:none;
      z-index:0;
      white-space:pre-wrap;
      text-align:center;
    }
    .watermark::after{
      content:"";
      position:fixed; inset:0;
      background:
        radial-gradient(1200px 500px at 80% 10%, rgba(245,196,0,.18), transparent 60%),
        radial-gradient(900px 500px at 15% 25%, rgba(245,196,0,.10), transparent 60%),
        radial-gradient(900px 600px at 50% 100%, rgba(255,255,255,.06), transparent 60%);
      pointer-events:none;
      z-index:0;
    }
    .content-layer{position:relative; z-index:1;}
    .glass{
      background:rgba(255,255,255,.06);
      border:1px solid rgba(255,255,255,.12);
      backdrop-filter: blur(10px);
    }
    .btn{
      display:inline-flex; align-items:center; justify-content:center;
      gap:.5rem;
      border-radius:14px;
      padding:.9rem 1rem;
      font-weight:800;
      transition:.2s ease;
      white-space:nowrap;
    }
    .btn-primary{
      background:var(--brand-yellow);
      color:#111;
      box-shadow:0 10px 30px rgba(245,196,0,.22);
    }
    .btn-primary:hover{transform:translateY(-1px)}
    .btn-dark{
      background:rgba(255,255,255,.08);
      color:#fff;
      border:1px solid rgba(255,255,255,.14);
    }
    .btn-dark:hover{background:rgba(255,255,255,.11)}
    .chip{
      display:inline-flex; align-items:center; gap:.5rem;
      padding:.45rem .7rem; border-radius:999px;
      background:rgba(245,196,0,.12);
      border:1px solid rgba(245,196,0,.25);
      color:#fff;
      font-weight:800;
    }
    .badge{
      display:inline-flex; align-items:center; justify-content:center;
      padding:.25rem .55rem; border-radius:999px;
      background:rgba(255,255,255,.08);
      border:1px solid rgba(255,255,255,.14);
      color:#fff;
      font-weight:800;
      font-size:.85rem;
    }
    .section-title{
      font-weight:900;
      letter-spacing:.2px;
    }
    /* Top urgent bar */
    .ticker{
      background:linear-gradient(90deg, rgba(245,196,0,.95), rgba(245,196,0,.75));
      color:#111;
    }
    /* Toast */
    .toast{
      position:fixed;
      bottom:16px; left:16px;
      max-width:min(360px, calc(100vw - 32px));
      z-index:80;
      display:none;
    }
    /* Modal */
    .modal-backdrop{display:none}
    .modal-backdrop.active{display:block}
    /* Mobile menu */
    .drawer{transform:translateY(-8px); opacity:0; pointer-events:none}
    .drawer.active{transform:translateY(0); opacity:1; pointer-events:auto}
  </style>
</head>

<body class="watermark text-white">
  <div class="content-layer">

    <!-- Sticky urgent bar -->
    <div class="ticker w-full text-sm md:text-base font-extrabold px-4 py-2 text-center sticky top-0 z-50">
      🚨 التسجيل ينتهي <span class="underline">29/01/2026</span> أو عند اكتمال العدد — السعر بعد الإغلاق <span class="line-through">449</span> <span class="font-black">ريال</span>
      <span class="mx-2">|</span>
      الخصم الحالي: <span class="font-black">299 ريال</span>
    </div>

    <!-- Header -->
    <header class="px-4 pt-5">
      <div class="max-w-6xl mx-auto glass rounded-2xl px-4 py-4">
        <div class="flex items-center justify-between gap-3">
          <div class="flex items-center gap-3">
            <div class="h-11 w-11 rounded-2xl flex items-center justify-center" style="background:rgba(245,196,0,.18);border:1px solid rgba(245,196,0,.30)">
              <span class="text-xl font-black" style="color:var(--brand-yellow)">A</span>
            </div>
            <div class="leading-tight">
              <div class="font-black text-lg md:text-xl">أكاديمية عايد الرسمية</div>
              <div class="text-white/70 font-bold text-sm md:text-base">دورة STEP المكثفة 2026 — أونلاين</div>
            </div>
          </div>

          <div class="hidden md:flex items-center gap-2">
            <a href="#pricing" class="btn btn-primary">اشترك الآن</a>
            <a href="#contact" class="btn btn-dark">تواصل</a>
            <button id="shareBtn" class="btn btn-dark">مشاركة الإعلان</button>
          </div>

          <button id="menuBtn" class="md:hidden btn btn-dark px-3">القائمة</button>
        </div>

        <!-- Desktop TOC -->
        <nav class="hidden md:flex flex-wrap items-center gap-2 mt-4">
          <a class="badge hover:bg-white/10" href="#about">عن الدورة</a>
          <a class="badge hover:bg-white/10" href="#features">المميزات</a>
          <a class="badge hover:bg-white/10" href="#content">المحتوى</a>
          <a class="badge hover:bg-white/10" href="#plan15">خطة 15 يوم</a>
          <a class="badge hover:bg-white/10" href="#pricing">السعر والدفع</a>
          <a class="badge hover:bg-white/10" href="#enroll">التسجيل</a>
          <a class="badge hover:bg-white/10" href="#reviews">نتائج الطلاب</a>
          <a class="badge hover:bg-white/10" href="#faq">الأسئلة</a>
          <a class="badge hover:bg-white/10" href="#contact">التواصل</a>
        </nav>

        <!-- Mobile Drawer -->
        <nav id="drawer" class="drawer md:hidden mt-3 grid grid-cols-2 gap-2 transition-all duration-200">
          <a class="badge justify-center" href="#about">عن الدورة</a>
          <a class="badge justify-center" href="#features">المميزات</a>
          <a class="badge justify-center" href="#content">المحتوى</a>
          <a class="badge justify-center" href="#plan15">خطة 15 يوم</a>
          <a class="badge justify-center" href="#pricing">السعر والدفع</a>
          <a class="badge justify-center" href="#enroll">التسجيل</a>
          <a class="badge justify-center" href="#reviews">نتائج الطلاب</a>
          <a class="badge justify-center" href="#faq">الأسئلة</a>
          <a class="badge justify-center" href="#contact">التواصل</a>
          <button class="btn btn-primary col-span-2" onclick="document.querySelector('#pricing').scrollIntoView({behavior:'smooth'})">اشترك الآن</button>
          <button class="btn btn-dark col-span-2" id="shareBtnMobile">مشاركة الإعلان</button>
        </nav>
      </div>
    </header>

    <!-- Hero -->
    <section class="px-4 mt-5">
      <div class="max-w-6xl mx-auto grid lg:grid-cols-2 gap-4">
        <div class="glass rounded-3xl p-6 md:p-8">
          <div class="flex flex-wrap items-center gap-2">
            <span class="chip">✅ تحديثات 2026 حسب قياس</span>
            <span class="chip">🧠 محتوى مركز بدون تشتت</span>
            <span class="chip">📌 نموذج 50 + (قريبًا 51)</span>
          </div>

          <h1 class="mt-4 text-3xl md:text-5xl font-black leading-tight">
            جهّز نفسك لـ STEP خلال وقت قصير
            <span style="color:var(--brand-yellow)">وبخطة واضحة</span>
          </h1>

          <p class="mt-4 text-white/80 text-lg font-bold leading-relaxed">
            هذه دورة عملية ومكثفة للي اختبارهم قريب أو يبون يرفعون الدرجة بسرعة.
            بنمشي معك خطوة بخطوة: شرح + تدريب + نماذج حديثة + خطة مذاكرة جاهزة.
          </p>

          <div class="mt-6 grid sm:grid-cols-3 gap-3">
            <div class="glass rounded-2xl p-4">
              <div class="text-white/70 font-extrabold">السعر الحالي</div>
              <div class="text-2xl font-black mt-1"><span style="color:var(--brand-yellow)">299</span> ريال</div>
              <div class="text-white/60 font-bold mt-1">بعد الإغلاق: <span class="line-through">449</span></div>
            </div>
            <div class="glass rounded-2xl p-4">
              <div class="text-white/70 font-extrabold">مدة الوصول</div>
              <div class="text-2xl font-black mt-1">90 يوم</div>
              <div class="text-white/60 font-bold mt-1">+ دعم فني خلال المدة</div>
            </div>
            <div class="glass rounded-2xl p-4">
              <div class="text-white/70 font-extrabold">ينتهي التسجيل خلال</div>
              <div class="text-2xl font-black mt-1" id="countdown">—</div>
              <div class="text-white/60 font-bold mt-1">29/01/2026</div>
            </div>
          </div>

          <div class="mt-6 flex flex-wrap gap-2">
            <button class="btn btn-primary" onclick="document.querySelector('#pricing').scrollIntoView({behavior:'smooth'})">ابدأ الاشتراك الآن</button>
            <button class="btn btn-dark" onclick="document.querySelector('#plan15').scrollIntoView({behavior:'smooth'})">شوف خطة 15 يوم</button>
            <button class="btn btn-dark" id="shareBtnHero">مشاركة الإعلان</button>
          </div>

          <div class="mt-6 flex flex-wrap items-center gap-2 text-white/75 font-bold">
            <span class="badge">🔔 يتم تفعيل الطلب بعد مراجعة الإيصال</span>
            <span class="badge">🛡️ التحويل فقط على البيانات الرسمية أدناه</span>
          </div>
        </div>

        <div class="glass rounded-3xl p-6 md:p-8">
          <div class="flex items-center justify-between">
            <h2 class="section-title text-2xl md:text-3xl">نشاط الأكاديمية</h2>
            <span class="badge">تجريبي (قابل للتعديل)</span>
          </div>

          <div class="mt-4 grid sm:grid-cols-2 gap-3">
            <div class="glass rounded-2xl p-4">
              <div class="text-white/70 font-extrabold">طلبات اليوم</div>
              <div class="text-3xl font-black mt-1" id="liveRequests">17</div>
              <div class="text-white/60 font-bold mt-1">يتحدث تلقائيًا</div>
            </div>
            <div class="glass rounded-2xl p-4">
              <div class="text-white/70 font-extrabold">مقاعد متبقية (تقديري)</div>
              <div class="text-3xl font-black mt-1" id="seatsLeft">62</div>
              <div class="text-white/60 font-bold mt-1">يتغير حسب الإقبال</div>
            </div>
          </div>

          <div class="mt-4 glass rounded-2xl p-4">
            <div class="flex items-center justify-between">
              <div class="font-black text-lg">ليش الناس تختار المكثفة؟</div>
              <div class="text-white/60 font-bold">مختصر ومفيد</div>
            </div>
            <ul class="mt-3 space-y-2 text-white/80 font-bold">
              <li>• ترتيب المحتوى من التمهيدي إلى النماذج بشكل واضح.</li>
              <li>• تركيز على النقاط المتكررة في الاختبار + استراتيجيات الحل.</li>
              <li>• ملفات ونماذج عملية + متابعة.</li>
              <li>• مناسب للي يبي نتيجة بسرعة بدون تشتيت دورات ومصادر.</li>
            </ul>
          </div>

          <div class="mt-4 flex flex-wrap gap-2">
            <a class="btn btn-dark" href="https://t.me/Academy_Ayed_2026" target="_blank" rel="noopener">قروب التنبيهات الرسمي</a>
            <a class="btn btn-dark" href="https://t.me/ayedacadmeybot" target="_blank" rel="noopener">بوت المحتوى المجاني</a>
            <a class="btn btn-primary" href="https://t.me/Ayed_Academy_2026" target="_blank" rel="noopener">الحساب الرسمي للاشتراك</a>
          </div>

          <p class="mt-4 text-white/60 font-bold text-sm leading-relaxed">
            ملاحظة: الأرقام/الإشعارات هنا للتصميم (تقدر تعدلها لبياناتك الفعلية). الأهم: التفعيل الرسمي يكون بعد مراجعة الإيصال عبر الحساب الرسمي.
          </p>
        </div>
      </div>
    </section>

    <!-- About -->
    <section id="about" class="px-4 mt-6">
      <div class="max-w-6xl mx-auto glass rounded-3xl p-6 md:p-8">
        <h2 class="section-title text-2xl md:text-3xl">عن دورة STEP المكثفة 2026</h2>
        <p class="mt-3 text-white/80 font-bold leading-relaxed">
          الدورة المكثفة مصممة لطلاب STEP اللي ودّهم يختصرون الطريق: بدل ما تتنقل بين مصادر كثيرة وأسعار مبالغ فيها وتضيع وقتك،
          هنا بتلقى محتوى مرتب ومركز على اللي يرفع درجتك فعلاً — وبأسلوب واضح يناسب وقتك واختبارك.
        </p>

        <div class="mt-5 grid md:grid-cols-3 gap-3">
          <div class="glass rounded-2xl p-4">
            <div class="font-black text-lg">🎯 الهدف</div>
            <div class="text-white/75 font-bold mt-1">رفع الدرجة بسرعة بخطة مختصرة + تدريب عملي.</div>
          </div>
          <div class="glass rounded-2xl p-4">
            <div class="font-black text-lg">🧩 مناسب لـ</div>
            <div class="text-white/75 font-bold mt-1">اللي اختبارهم قريب / اللي تشتتوا من المصادر / اللي يبون نماذج حديثة.</div>
          </div>
          <div class="glass rounded-2xl p-4">
            <div class="font-black text-lg">🛡️ ضمان التنظيم</div>
            <div class="text-white/75 font-bold mt-1">فهرسة واضحة + خطوات دفع/تسجيل مرتبة بدون لخبطة.</div>
          </div>
        </div>
      </div>
    </section>

    <!-- Features -->
    <section id="features" class="px-4 mt-6">
      <div class="max-w-6xl mx-auto grid lg:grid-cols-3 gap-4">
        <div class="glass rounded-3xl p-6 md:p-8 lg:col-span-2">
          <h2 class="section-title text-2xl md:text-3xl">مميزات الدورة (وش بتاخذ؟)</h2>
          <div class="mt-4 grid sm:grid-cols-2 gap-3 text-white/85 font-bold">
            <div class="glass rounded-2xl p-4">✅ شرح وتدريب مركز على الأقسام الأساسية</div>
            <div class="glass rounded-2xl p-4">📌 نماذج حديثة (نموذج 50) + تحديثات مستمرة</div>
            <div class="glass rounded-2xl p-4">🗂️ ملفات مرتبة + نماذج PDF جاهزة</div>
            <div class="glass rounded-2xl p-4">🧠 استراتيجيات للحل وتوفير الوقت داخل الاختبار</div>
            <div class="glass rounded-2xl p-4">🗓️ خطة مذاكرة (15 يوم) + تقدر تعدلها حسب وقتك</div>
            <div class="glass rounded-2xl p-4">📩 تفعيل ودعم عبر الحساب الرسمي خلال فترة الاشتراك</div>
          </div>
        </div>

        <div class="glass rounded-3xl p-6 md:p-8">
          <h3 class="section-title text-xl md:text-2xl">تنبيه مهم ضد الاحتيال</h3>
          <p class="mt-3 text-white/80 font-bold leading-relaxed">
            أي تحويل خارج بيانات التحويل الرسمية في هذه الصفحة غير معتمد.
            التفعيل يتم فقط بعد إرسال الإيصال للحساب الرسمي:
          </p>
          <div class="mt-4 flex flex-wrap gap-2">
            <a class="btn btn-primary w-full" href="https://t.me/Ayed_Academy_2026" target="_blank" rel="noopener">👉 @Ayed_Academy_2026</a>
            <a class="btn btn-dark w-full" href="https://t.me/Academy_Ayed_2026" target="_blank" rel="noopener">قروب التنبيهات الرسمي</a>
          </div>
        </div>
      </div>
    </section>

    <!-- Content -->
    <section id="content" class="px-4 mt-6">
      <div class="max-w-6xl mx-auto glass rounded-3xl p-6 md:p-8">
        <h2 class="section-title text-2xl md:text-3xl">محتوى الدورة (مختصر وواضح)</h2>

        <div class="mt-4 grid md:grid-cols-3 gap-3 text-white/85 font-bold">
          <div class="glass rounded-2xl p-5">
            <div class="font-black text-xl">📌 التمهيدي</div>
            <ul class="mt-2 space-y-2 text-white/80 font-bold">
              <li>• مناسب للي يحس مستواه يحتاج شدّة.</li>
              <li>• خطوة اختيارية قبل الدخول للمكثف.</li>
            </ul>
          </div>
          <div class="glass rounded-2xl p-5">
            <div class="font-black text-xl">🔵 Grammar (القواعد)</div>
            <ul class="mt-2 space-y-2 text-white/80 font-bold">
              <li>• تأسيس سريع على النقاط المتكررة.</li>
              <li>• تدريب على المودلز (نماذج) بشكل مرتب.</li>
              <li>• كويزات ومراجعات تثبيت.</li>
            </ul>
          </div>
          <div class="glass rounded-2xl p-5">
            <div class="font-black text-xl">🟣 Reading (القراءة)</div>
            <ul class="mt-2 space-y-2 text-white/80 font-bold">
              <li>• استراتيجيات استخراج الإجابة بسرعة.</li>
              <li>• نماذج واقعية متعددة.</li>
              <li>• مراجعات + تدريب.</li>
            </ul>
          </div>
          <div class="glass rounded-2xl p-5 md:col-span-3">
            <div class="font-black text-xl">⚪ Listening (الاستماع)</div>
            <div class="grid md:grid-cols-3 gap-3 mt-2">
              <div class="glass rounded-2xl p-4">
                <div class="font-black">استراتيجيات</div>
                <div class="text-white/80 font-bold mt-1">كيف تلتقط الفكرة بسرعة وتختصر وقتك.</div>
              </div>
              <div class="glass rounded-2xl p-4">
                <div class="font-black">تدريب يومي</div>
                <div class="text-white/80 font-bold mt-1">نصف ساعة يوميًا كفاية مع الاستمرارية.</div>
              </div>
              <div class="glass rounded-2xl p-4">
                <div class="font-black">نموذج 50 + تحديث 51</div>
                <div class="text-white/80 font-bold mt-1">نركز على أحدث النماذج، والجديد ينزل أول بأول.</div>
              </div>
            </div>
          </div>
        </div>

        <div class="mt-5 flex flex-wrap gap-2">
          <button class="btn btn-dark" onclick="document.querySelector('#plan15').scrollIntoView({behavior:'smooth'})">الانتقال لخطة 15 يوم</button>
          <button class="btn btn-primary" onclick="document.querySelector('#pricing').scrollIntoView({behavior:'smooth'})">روح للدفع والتسجيل</button>
        </div>
      </div>
    </section>

    <!-- 15-day plan -->
    <section id="plan15" class="px-4 mt-6">
      <div class="max-w-6xl mx-auto glass rounded-3xl p-6 md:p-8">
        <div class="flex flex-wrap items-center justify-between gap-2">
          <h2 class="section-title text-2xl md:text-3xl">خطة مذاكرة STEP (15 يوم)</h2>
          <span class="badge">مبنية على جدول: قراءة + قرامر + استماع</span>
        </div>

        <p class="mt-3 text-white/80 font-bold leading-relaxed">
          الخطة بسيطة وواضحة: كل يوم <span class="font-black" style="color:var(--brand-yellow)">مجموعتين نماذج</span> في القرامر + نفس المجموعتين في الريدنق،
          ومعهم <span class="font-black">نصف ساعة استماع</span>. (تقدر تزيد/تقلل حسب وقتك).
        </p>

        <div class="mt-4 grid lg:grid-cols-3 gap-3 text-white/85 font-bold">
          <div class="glass rounded-2xl p-5">
            <div class="font-black text-xl">🟣 Reading (15 يوم)</div>
            <ol class="mt-3 space-y-2 text-white/80 font-bold list-decimal pr-5">
              <li>نماذج 5–7</li>
              <li>نماذج 8–10</li>
              <li>نماذج 11–14</li>
              <li>نماذج 15–17</li>
              <li>نماذج 18–20</li>
              <li>نماذج 21–23</li>
              <li>نماذج 24–26</li>
              <li>نماذج 27–29</li>
              <li>نماذج 30–32</li>
              <li>نماذج 33–35</li>
              <li>نماذج 36–38</li>
              <li>نماذج 39–41</li>
              <li>نماذج 42–44</li>
              <li>نماذج 45–47</li>
              <li>نموذج 48–50</li>
            </ol>
          </div>

          <div class="glass rounded-2xl p-5">
            <div class="font-black text-xl">🔵 Grammar (15 يوم)</div>
            <ol class="mt-3 space-y-2 text-white/80 font-bold list-decimal pr-5">
              <li>نماذج 5–7</li>
              <li>نماذج 8–10</li>
              <li>نماذج 11–14</li>
              <li>نماذج 15–17</li>
              <li>نماذج 18–20</li>
              <li>نماذج 21–23</li>
              <li>نماذج 24–26</li>
              <li>نماذج 27–29</li>
              <li>نماذج 30–32</li>
              <li>نماذج 33–35</li>
              <li>نماذج 36–38</li>
              <li>نماذج 39–41</li>
              <li>نماذج 42–44</li>
              <li>نماذج 45–47</li>
              <li>نموذج 48–50</li>
            </ol>
          </div>

          <div class="glass rounded-2xl p-5">
            <div class="font-black text-xl">⚪ Listening (يومي)</div>
            <div class="mt-3 text-white/80 font-bold leading-relaxed">
              <div class="glass rounded-2xl p-4">
                ✅ كل يوم: <span class="font-black" style="color:var(--brand-yellow)">30 دقيقة استماع</span><br/>
                <span class="text-white/70 font-bold">ركز على نوعية الأسئلة + الكلمات المتكررة + مراجعة الغلط.</span>
              </div>
              <div class="mt-3 glass rounded-2xl p-4">
                نصيحة: إذا واجهت سؤال ما قدرت عليه — <span class="font-black">ترجمه</span> وفهم الفكرة، وارجع له مرة ثانية.
              </div>
              <div class="mt-3 glass rounded-2xl p-4">
                بعد ما تخلص: راجع <span class="font-black">الأكثر تكرار</span> كمرحلة تعزيز نهائية.
              </div>
            </div>
          </div>
        </div>

        <div class="mt-5 flex flex-wrap gap-2">
          <button class="btn btn-dark" onclick="document.querySelector('#pricing').scrollIntoView({behavior:'smooth'})">جاهز؟ روح للدفع</button>
          <button class="btn btn-primary" onclick="document.querySelector('#enroll').scrollIntoView({behavior:'smooth'})">فتح نموذج التسجيل</button>
        </div>
      </div>
    </section>

    <!-- Pricing + Payment -->
    <section id="pricing" class="px-4 mt-6">
      <div class="max-w-6xl mx-auto grid lg:grid-cols-2 gap-4">
        <div class="glass rounded-3xl p-6 md:p-8">
          <h2 class="section-title text-2xl md:text-3xl">السعر وطريقة الدفع</h2>

          <div class="mt-4 glass rounded-2xl p-5">
            <div class="flex flex-wrap items-center gap-2">
              <span class="chip">💵 السعر الحالي: 299 ريال</span>
              <span class="chip">⏳ ينتهي: 29/01/2026</span>
              <span class="chip">📌 بعد الإغلاق: 449 ريال</span>
            </div>
            <p class="mt-3 text-white/80 font-bold leading-relaxed">
              التسجيل يتفعل بعد مراجعة الإيصال عبر الحساب الرسمي. لا ترسل تحويل لأي جهة ثانية.
            </p>
          </div>

          <div class="mt-4 glass rounded-2xl p-5">
            <div class="font-black text-xl mb-2">📢 بيانات التحويل البنكي الرسمية</div>
            <div class="space-y-3 text-white/85 font-bold">
              <div class="flex flex-wrap items-center justify-between gap-2">
                <div>🟢 البنك: <span class="font-black">بنك الإنماء</span></div>
              </div>

              <div class="glass rounded-2xl p-4">
                <div class="flex items-center justify-between gap-2">
                  <div>🏦 رقم الحساب:</div>
                  <button class="btn btn-dark py-2 px-3 text-sm" onclick="copyText('68206067557000')">نسخ</button>
                </div>
                <div class="mt-1 text-xl font-black" dir="ltr">68206067557000</div>
              </div>

              <div class="glass rounded-2xl p-4">
                <div class="flex items-center justify-between gap-2">
                  <div>🏦 الآيبان:</div>
                  <button class="btn btn-dark py-2 px-3 text-sm" onclick="copyText('SA4905000068206067557000')">نسخ</button>
                </div>
                <div class="mt-1 text-xl font-black" dir="ltr">SA4905000068206067557000</div>
              </div>

              <div class="glass rounded-2xl p-4">
                <div class="flex items-center justify-between gap-2">
                  <div>👤 اسم المستفيد (عربي):</div>
                  <button class="btn btn-dark py-2 px-3 text-sm" onclick="copyText('مؤسسة كريتيفا جلوبال لتقنية المعلومات')">نسخ</button>
                </div>
                <div class="mt-1 text-lg font-black">مؤسسة كريتيفا جلوبال لتقنية المعلومات</div>
              </div>

              <div class="glass rounded-2xl p-4">
                <div class="flex items-center justify-between gap-2">
                  <div>📝 غرض التحويل (ضروري):</div>
                  <button class="btn btn-dark py-2 px-3 text-sm" onclick="copyText('مشتريات دورة STEP المكثفة – منصة عايد الرسمية')">نسخ</button>
                </div>
                <div class="mt-1 text-white/85 font-black">مشتريات دورة STEP المكثفة – منصة عايد الرسمية</div>
              </div>

              <div class="text-white/70 font-bold text-sm leading-relaxed">
                ملاحظة: إذا ظهر لك اسم مختصر عند التحويل فهذا طبيعي — المهم يكون على نفس رقم الحساب/الآيبان أعلاه.
              </div>
            </div>
          </div>

          <div class="mt-4 flex flex-wrap gap-2">
            <button class="btn btn-primary" onclick="document.querySelector('#enroll').scrollIntoView({behavior:'smooth'})">بعد التحويل؟ افتح نموذج التسجيل</button>
            <a class="btn btn-dark" href="https://t.me/Ayed_Academy_2026" target="_blank" rel="noopener">تواصل مباشر</a>
          </div>
        </div>

        <div class="glass rounded-3xl p-6 md:p-8">
          <h3 class="section-title text-2xl md:text-3xl">خطوات التسجيل (بدون لخبطة)</h3>

          <ol class="mt-4 space-y-3 text-white/85 font-bold">
            <li class="glass rounded-2xl p-4">1) حوّل <span style="color:var(--brand-yellow)" class="font-black">299 ريال</span> على البيانات الرسمية أعلاه.</li>
            <li class="glass rounded-2xl p-4">2) جهّز الإيصال (صورة أو PDF).</li>
            <li class="glass rounded-2xl p-4">3) عبّئ نموذج التسجيل تحت، وارفع الإيصال (إجباري).</li>
            <li class="glass rounded-2xl p-4">4) بعد الإرسال: بنفتح لك تلقائيًا رسالة جاهزة للحساب الرسمي — الصقها وأرسلها + <span class="font-black">أرفق الإيصال مرة ثانية</span> في تليجرام للتأكيد.</li>
            <li class="glass rounded-2xl p-4">5) خلال <span class="font-black">24 ساعة</span> يتم تفعيل طلبك وإرسال تعليمات البداية.</li>
          </ol>

          <div class="mt-4 glass rounded-2xl p-4 text-white/75 font-bold leading-relaxed">
            ✅ ملاحظة مهمة: الموقع ما يرفع ملفاتك لأي سيرفر (ستاتيك). الإيصال يستخدم للتأكد أنه موجود عندك فقط،
            والتأكيد الرسمي يكون بإرفاق الإيصال في تليجرام للحساب الرسمي.
          </div>

          <div class="mt-4 flex flex-wrap gap-2">
            <button class="btn btn-primary w-full" onclick="document.querySelector('#enroll').scrollIntoView({behavior:'smooth'})">ابدأ التسجيل الآن</button>
          </div>
        </div>
      </div>
    </section>

    <!-- Enroll Form -->
    <section id="enroll" class="px-4 mt-6">
      <div class="max-w-6xl mx-auto glass rounded-3xl p-6 md:p-8">
        <div class="flex flex-wrap items-center justify-between gap-2">
          <h2 class="section-title text-2xl md:text-3xl">نموذج التسجيل (بعد التحويل)</h2>
          <span class="badge">إرفاق الإيصال إجباري</span>
        </div>

        <form id="enrollForm" class="mt-5 grid md:grid-cols-2 gap-4 text-white/90 font-bold">
          <div class="glass rounded-2xl p-4">
            <label class="block mb-2">الاسم الثلاثي <span style="color:var(--brand-yellow)">*</span></label>
            <input id="fullName" type="text" class="w-full rounded-xl bg-white/10 border border-white/15 px-4 py-3 outline-none focus:border-yellow-300"
              placeholder="مثال: محمد عبدالعزيز عايد" required />
          </div>

          <div class="glass rounded-2xl p-4">
            <label class="block mb-2">موعد الاختبار</label>
            <select id="examWhen" class="w-full rounded-xl bg-white/10 border border-white/15 px-4 py-3 outline-none focus:border-yellow-300">
              <option value="لسا ما حجزت">لسا ما حجزت</option>
              <option value="خلال أسبوع">خلال أسبوع</option>
              <option value="خلال أسبوعين">خلال أسبوعين</option>
              <option value="خلال شهر">خلال شهر</option>
              <option value="تاريخ محدد">تاريخ محدد (اختره تحت)</option>
            </select>
            <input id="examDate" type="date" class="mt-3 w-full rounded-xl bg-white/10 border border-white/15 px-4 py-3 outline-none focus:border-yellow-300 hidden" />
          </div>

          <div class="glass rounded-2xl p-4">
            <label class="block mb-2">الدرجة المستهدفة</label>
            <input id="targetScore" type="number" min="0" max="100" class="w-full rounded-xl bg-white/10 border border-white/15 px-4 py-3 outline-none focus:border-yellow-300"
              placeholder="مثال: 70" />
          </div>

          <div class="glass rounded-2xl p-4">
            <label class="block mb-2">هل اختبرت STEP قبل؟</label>
            <div class="flex flex-wrap gap-3">
              <label class="flex items-center gap-2"><input type="radio" name="testedBefore" value="نعم" class="accent-yellow-300"> نعم</label>
              <label class="flex items-center gap-2"><input type="radio" name="testedBefore" value="لا" class="accent-yellow-300" checked> لا</label>
            </div>
            <input id="prevScore" type="number" min="0" max="100" class="mt-3 w-full rounded-xl bg-white/10 border border-white/15 px-4 py-3 outline-none focus:border-yellow-300 hidden"
              placeholder="إذا نعم: درجتك السابقة (اختياري)" />
          </div>

          <div class="glass rounded-2xl p-4">
            <label class="block mb-2">مستواك الحالي</label>
            <select id="level" class="w-full rounded-xl bg-white/10 border border-white/15 px-4 py-3 outline-none focus:border-yellow-300">
              <option value="ما أدري">ما أدري</option>
              <option value="مبتدئ">مبتدئ</option>
              <option value="متوسط">متوسط</option>
              <option value="متقدم">متقدم</option>
            </select>
          </div>

          <div class="glass rounded-2xl p-4">
            <label class="block mb-2">سبب دخول الاختبار / الهدف</label>
            <select id="purpose" class="w-full rounded-xl bg-white/10 border border-white/15 px-4 py-3 outline-none focus:border-yellow-300">
              <option value="تقديم جامعة">تقديم جامعة</option>
              <option value="وظيفة">وظيفة</option>
              <option value="ابتعاث / برنامج">ابتعاث / برنامج</option>
              <option value="رفع مستوى">رفع مستوى</option>
              <option value="غير ذلك">غير ذلك</option>
            </select>
          </div>

          <div class="glass rounded-2xl p-4 md:col-span-2">
            <label class="block mb-2">طريقة التواصل (اختياري) + لماذا؟</label>
            <div class="text-white/70 font-bold text-sm mb-3">
              إذا حطيت وسيلة تواصل يساعدنا نوصل لك بسرعة لو احتجنا توضيح في البيانات. (اختياري)
            </div>

            <div class="flex flex-wrap gap-3">
              <label class="flex items-center gap-2">
                <input type="radio" name="contactType" value="تليجرام" class="accent-yellow-300" checked> تليجرام
              </label>
              <label class="flex items-center gap-2">
                <input type="radio" name="contactType" value="واتساب" class="accent-yellow-300"> واتساب
              </label>
              <label class="flex items-center gap-2">
                <input type="radio" name="contactType" value="إيميل" class="accent-yellow-300"> إيميل
              </label>
            </div>

            <input id="contactValue" type="text" class="mt-3 w-full rounded-xl bg-white/10 border border-white/15 px-4 py-3 outline-none focus:border-yellow-300"
              placeholder="مثال: @username أو 05xxxxxxxx أو name@email.com (اختياري)" />
          </div>

          <div class="glass rounded-2xl p-4 md:col-span-2">
            <label class="block mb-2">ملاحظات (اختياري)</label>
            <textarea id="notes" rows="3" class="w-full rounded-xl bg-white/10 border border-white/15 px-4 py-3 outline-none focus:border-yellow-300"
              placeholder="مثال: اختبار قريب جدًا — أبغى خطة 7 أيام / عندي ضعف في الريدنق..."></textarea>
          </div>

          <div class="glass rounded-2xl p-4 md:col-span-2">
            <label class="block mb-2">إرفاق إيصال التحويل (إجباري) <span style="color:var(--brand-yellow)">*</span></label>
            <input id="receipt" type="file" accept="image/*,application/pdf" class="w-full" required />
            <div class="text-white/70 font-bold text-sm mt-2">
              بعد فتح تليجرام وإرسال الرسالة الجاهزة: <span class="font-black">أرفق الإيصال مرة ثانية</span> في الخاص للتأكيد النهائي.
            </div>
          </div>

          <div class="glass rounded-2xl p-4 md:col-span-2">
            <label class="flex items-start gap-2 cursor-pointer">
              <input id="agree" type="checkbox" class="mt-1 accent-yellow-300" required>
              <span class="text-white/80 font-bold">
                أقر أني حولت الرسوم على البيانات الرسمية أعلاه، وأفهم أن التفعيل يتم بعد مراجعة الإيصال عبر الحساب الرسمي.
              </span>
            </label>
          </div>

          <div class="md:col-span-2 flex flex-wrap gap-2">
            <button type="submit" class="btn btn-primary flex-1">إرسال الطلب للحساب الرسمي</button>
            <button type="button" class="btn btn-dark" onclick="document.querySelector('#pricing').scrollIntoView({behavior:'smooth'})">رجوع للدفع</button>
          </div>
        </form>

        <div id="afterSubmit" class="hidden mt-5 glass rounded-2xl p-5">
          <div class="font-black text-xl">✅ تم تجهيز رسالتك</div>
          <div class="text-white/80 font-bold mt-2 leading-relaxed">
            إذا ما انفتح تليجرام تلقائيًا، اضغط الزر تحت. وبعد ما تفتح المحادثة:
            <span class="font-black">أرسل الرسالة</span> ثم <span class="font-black">أرفق الإيصال مرة ثانية</span> وأرسله.
          </div>
          <div class="mt-4 flex flex-wrap gap-2">
            <a id="tgLink" class="btn btn-primary" href="#" target="_blank" rel="noopener">فتح محادثة الأكاديمية</a>
            <a class="btn btn-dark" href="https://t.me/Ayed_Academy_2026" target="_blank" rel="noopener">فتح بدون رسالة جاهزة</a>
          </div>
        </div>
      </div>
    </section>

    <!-- Reviews -->
    <section id="reviews" class="px-4 mt-6">
      <div class="max-w-6xl mx-auto glass rounded-3xl p-6 md:p-8">
        <h2 class="section-title text-2xl md:text-3xl">نتائج وآراء طلاب (نماذج قابلة للتعديل)</h2>
        <div class="mt-4 grid md:grid-cols-3 gap-3 text-white/85 font-bold">
          <div class="glass rounded-2xl p-5">
            <div class="font-black">ريم</div>
            <div class="text-white/75 mt-2">رفعت درجتي من 49 إلى 66 خلال شهر، التنظيم فرق معي جدًا.</div>
          </div>
          <div class="glass rounded-2xl p-5">
            <div class="font-black">عبدالله</div>
            <div class="text-white/75 mt-2">الدورة مختصرة وما فيها تشتت، ركزت على النماذج والنتيجة طلعت.</div>
          </div>
          <div class="glass rounded-2xl p-5">
            <div class="font-black">سارة</div>
            <div class="text-white/75 mt-2">خطة 15 يوم ساعدتني ألتزم، خصوصًا الاستماع اليومي.</div>
          </div>
        </div>

        <div class="mt-5 glass rounded-2xl p-5">
          <div class="font-black text-xl">تبغى تضيف نتائج حقيقية؟</div>
          <div class="text-white/75 font-bold mt-2">
            عدّل النصوص هنا أو ضيف صور/سكرينات (مع طمس البيانات الحساسة) عشان تزيد المصداقية.
          </div>
        </div>
      </div>
    </section>

    <!-- FAQ -->
    <section id="faq" class="px-4 mt-6">
      <div class="max-w-6xl mx-auto glass rounded-3xl p-6 md:p-8">
        <h2 class="section-title text-2xl md:text-3xl">الأسئلة الشائعة</h2>

        <div class="mt-4 grid md:grid-cols-2 gap-3 text-white/85 font-bold">
          <div class="glass rounded-2xl p-5">
            <div class="font-black">هل النماذج لحالها تكفي؟</div>
            <div class="text-white/75 mt-2">النماذج مهمة جدًا، لكن الأفضل تمشي مع الاستراتيجيات والمراجعة والكويزات عشان تثبت الفهم.</div>
          </div>
          <div class="glass rounded-2xl p-5">
            <div class="font-black">متى يتفعل اشتراكي؟</div>
            <div class="text-white/75 mt-2">بعد إرسال الإيصال للحساب الرسمي ومراجعته — عادة خلال 24 ساعة.</div>
          </div>
          <div class="glass rounded-2xl p-5">
            <div class="font-black">مدة الوصول؟</div>
            <div class="text-white/75 mt-2">90 يوم من تاريخ التفعيل + دعم فني خلال الفترة.</div>
          </div>
          <div class="glass rounded-2xl p-5">
            <div class="font-black">ليش السعر بيرتفع بعد 29/01؟</div>
            <div class="text-white/75 mt-2">لأننا بنقفل التسجيل على عدد محدد، وبعدها يفتح بسعره الرسمي (449 ريال).</div>
          </div>
        </div>
      </div>
    </section>

    <!-- Contact -->
    <section id="contact" class="px-4 mt-6 mb-10">
      <div class="max-w-6xl mx-auto glass rounded-3xl p-6 md:p-8">
        <h2 class="section-title text-2xl md:text-3xl">التواصل الرسمي</h2>

        <div class="mt-4 grid md:grid-cols-3 gap-3 text-white/85 font-bold">
          <a class="glass rounded-2xl p-5 hover:bg-white/10 transition" href="https://t.me/Ayed_Academy_2026" target="_blank" rel="noopener">
            <div class="font-black text-xl">📩 الحساب الرسمي</div>
            <div class="text-white/75 mt-2">@Ayed_Academy_2026</div>
          </a>
          <a class="glass rounded-2xl p-5 hover:bg-white/10 transition" href="https://t.me/Academy_Ayed_2026" target="_blank" rel="noopener">
            <div class="font-black text-xl">📢 قروب التنبيهات</div>
            <div class="text-white/75 mt-2">تحديثات + عروض + خطط مذاكرة</div>
          </a>
          <a class="glass rounded-2xl p-5 hover:bg-white/10 transition" href="https://t.me/ayedacadmeybot" target="_blank" rel="noopener">
            <div class="font-black text-xl">🤖 بوت مجاني</div>
            <div class="text-white/75 mt-2">تجميعات/كويزات منصة عايد المجانية</div>
          </a>
        </div>

        <div class="mt-5 flex flex-wrap items-center justify-between gap-2 text-white/70 font-bold">
          <div>© 2026 أكاديمية عايد — جميع الحقوق محفوظة</div>
          <div class="flex gap-3">
            <button class="underline hover:text-white" onclick="openModal('privacyModal')">سياسة الخصوصية</button>
            <button class="underline hover:text-white" onclick="openModal('reportModal')">بلاغ/احتيال</button>
          </div>
        </div>
      </div>
    </section>

    <!-- Floating actions -->
    <div class="fixed right-4 bottom-4 z-50 flex flex-col gap-2">
      <button class="btn btn-primary shadow-lg" onclick="document.querySelector('#pricing').scrollIntoView({behavior:'smooth'})">اشترك الآن</button>
      <a class="btn btn-dark" href="https://t.me/Ayed_Academy_2026" target="_blank" rel="noopener">تواصل</a>
    </div>

    <!-- Toast -->
    <div id="toast" class="toast glass rounded-2xl p-4">
      <div class="flex items-start gap-3">
        <div class="h-10 w-10 rounded-2xl flex items-center justify-center" style="background:rgba(245,196,0,.18);border:1px solid rgba(245,196,0,.30)">
          <span class="font-black" style="color:var(--brand-yellow)">✓</span>
        </div>
        <div class="flex-1">
          <div id="toastTitle" class="font-black"></div>
          <div id="toastText" class="text-white/75 font-bold mt-1"></div>
          <div class="text-white/50 font-bold text-xs mt-2">إشعار (تجريبي) — عدّل النصوص حسب بياناتك</div>
        </div>
        <button class="text-white/70 font-black" onclick="hideToast()">×</button>
      </div>
    </div>

    <!-- Modals -->
    <div id="privacyModal" class="modal-backdrop fixed inset-0 z-[90] bg-black/70 p-4">
      <div class="max-w-xl mx-auto mt-10 glass rounded-3xl p-6">
        <div class="flex items-center justify-between">
          <div class="font-black text-xl">سياسة الخصوصية</div>
          <button class="btn btn-dark py-2 px-3" onclick="closeModal('privacyModal')">إغلاق</button>
        </div>
        <div class="mt-3 text-white/80 font-bold leading-relaxed">
          • هذه الصفحة لا تخزن بياناتك في سيرفر ولا ترفع الإيصال.<br/>
          • الإيصال يكون عندك، والتأكيد الرسمي يتم بإرفاقه في تليجرام للحساب الرسمي.<br/>
          • أي بيانات تدخلها هنا تُستخدم فقط لتجهيز رسالة جاهزة لك لتسريع التسجيل.
        </div>
      </div>
    </div>

    <div id="reportModal" class="modal-backdrop fixed inset-0 z-[90] bg-black/70 p-4">
      <div class="max-w-xl mx-auto mt-10 glass rounded-3xl p-6">
        <div class="flex items-center justify-between">
          <div class="font-black text-xl">بلاغ / احتيال</div>
          <button class="btn btn-dark py-2 px-3" onclick="closeModal('reportModal')">إغلاق</button>
        </div>
        <div class="mt-3 text-white/80 font-bold leading-relaxed">
          إذا وصلك طلب تحويل من جهة غير الحساب الرسمي أو بيانات مختلفة — لا تحول.<br/>
          بلّغنا مباشرة عبر: <a class="underline" href="https://t.me/Ayed_Academy_2026" target="_blank" rel="noopener">@Ayed_Academy_2026</a>
        </div>
      </div>
    </div>

    <!-- Share Modal (fallback) -->
    <div id="shareModal" class="modal-backdrop fixed inset-0 z-[90] bg-black/70 p-4">
      <div class="max-w-xl mx-auto mt-10 glass rounded-3xl p-6">
        <div class="flex items-center justify-between">
          <div class="font-black text-xl">مشاركة إعلان الدورة</div>
          <button class="btn btn-dark py-2 px-3" onclick="closeModal('shareModal')">إغلاق</button>
        </div>
        <div class="mt-3 text-white/80 font-bold leading-relaxed">
          اختر المكان اللي تبي تشارك فيه (بيطلع لك نص جاهز):
        </div>
        <div class="mt-4 grid sm:grid-cols-2 gap-2">
          <a id="shareWa" class="btn btn-primary" href="#" target="_blank" rel="noopener">واتساب</a>
          <a id="shareTg" class="btn btn-dark" href="#" target="_blank" rel="noopener">تليجرام</a>
          <button class="btn btn-dark sm:col-span-2" onclick="copyText(getShareText())">نسخ نص الإعلان</button>
        </div>
      </div>
    </div>

  </div>

  <script>
    // ====== Settings ======
    const OFFICIAL_USERNAME = "Ayed_Academy_2026";
    const ENROLL_DEADLINE = new Date("2026-01-29T23:59:59+03:00");

    // ====== Countdown ======
    const countdownEl = document.getElementById("countdown");
    function pad(n){ return String(n).padStart(2,"0"); }
    function tickCountdown(){
      const now = new Date();
      const diff = ENROLL_DEADLINE - now;
      if(diff <= 0){
        countdownEl.textContent = "انتهى";
        return;
      }
      const s = Math.floor(diff/1000);
      const days = Math.floor(s/86400);
      const hours = Math.floor((s%86400)/3600);
      const mins = Math.floor((s%3600)/60);
      const secs = s%60;
      countdownEl.textContent = `${days}ي ${pad(hours)}:${pad(mins)}:${pad(secs)}`;
    }
    tickCountdown();
    setInterval(tickCountdown, 1000);

    // ====== Copy ======
    async function copyText(text){
      try{
        await navigator.clipboard.writeText(text);
        showToast("تم النسخ ✅", text);
      }catch(e){
        const ta = document.createElement("textarea");
        ta.value = text; document.body.appendChild(ta);
        ta.select(); document.execCommand("copy");
        document.body.removeChild(ta);
        showToast("تم النسخ ✅", text);
      }
    }

    // ====== Mobile menu ======
    const menuBtn = document.getElementById("menuBtn");
    const drawer = document.getElementById("drawer");
    if(menuBtn){
      menuBtn.addEventListener("click", ()=> drawer.classList.toggle("active"));
      drawer.querySelectorAll("a").forEach(a => a.addEventListener("click", ()=>drawer.classList.remove("active")));
    }

    // ====== Exam date logic ======
    const examWhen = document.getElementById("examWhen");
    const examDate = document.getElementById("examDate");
    examWhen.addEventListener("change", ()=>{
      if(examWhen.value === "تاريخ محدد"){
        examDate.classList.remove("hidden");
      }else{
        examDate.classList.add("hidden");
        examDate.value = "";
      }
    });

    // ====== Tested before logic ======
    const prevScore = document.getElementById("prevScore");
    document.querySelectorAll('input[name="testedBefore"]').forEach(r=>{
      r.addEventListener("change", ()=>{
        const val = document.querySelector('input[name="testedBefore"]:checked')?.value || "لا";
        if(val === "نعم") prevScore.classList.remove("hidden");
        else { prevScore.classList.add("hidden"); prevScore.value=""; }
      });
    });

    // ====== Form submit -> open Telegram deep link ======
    const form = document.getElementById("enrollForm");
    const afterSubmit = document.getElementById("afterSubmit");
    const tgLink = document.getElementById("tgLink");

    function buildMessage(data){
      const lines = [
        "السلام عليكم ورحمة الله وبركاته،",
        "أنا أرسلت إيصال التحويل لتأكيد اشتراكي في:",
        "✅ دورة STEP المكثفة 2026 (أكاديمية عايد الرسمية)",
        "",
        "📌 بياناتي:",
        `• الاسم: ${data.fullName}`,
        `• موعد الاختبار: ${data.examInfo}`,
        `• الدرجة المستهدفة: ${data.targetScore || "—"}`,
        `• هل اختبرت قبل؟: ${data.testedBefore}${data.prevScore ? " | الدرجة السابقة: " + data.prevScore : ""}`,
        `• المستوى: ${data.level}`,
        `• الهدف من الاختبار: ${data.purpose}`,
        data.contactValue ? `• وسيلة التواصل (${data.contactType}): ${data.contactValue}` : "• وسيلة التواصل: (لم يتم إدخالها)",
        data.notes ? `• ملاحظات: ${data.notes}` : "• ملاحظات: —",
        "",
        "🧾 الإيصال:",
        `• اسم الملف: ${data.receiptName}`,
        "",
        "✅ تم التحويل على البيانات الرسمية المذكورة في الموقع.",
        "الرجاء تأكيد الحجز وتفعيل اشتراكي،",
        "وبإذن الله أرفق الإيصال هنا مرة ثانية في الخاص للتأكيد النهائي.",
        "",
        "جزاكم الله خير."
      ];
      return lines.join("\n");
    }

    form.addEventListener("submit", (e)=>{
      e.preventDefault();

      const receipt = document.getElementById("receipt").files?.[0];
      if(!receipt){
        alert("لازم ترفق الإيصال (صورة أو PDF) قبل الإرسال.");
        return;
      }

      const fullName = document.getElementById("fullName").value.trim();
      if(!fullName){
        alert("اكتب اسمك الثلاثي.");
        return;
      }

      const testedBefore = document.querySelector('input[name="testedBefore"]:checked')?.value || "لا";
      const prev = document.getElementById("prevScore").value.trim();

      const examInfo = (examWhen.value === "تاريخ محدد" && examDate.value)
        ? examDate.value
        : examWhen.value;

      const contactType = document.querySelector('input[name="contactType"]:checked')?.value || "تليجرام";
      const contactValue = document.getElementById("contactValue").value.trim();

      const data = {
        fullName,
        examInfo,
        targetScore: document.getElementById("targetScore").value.trim(),
        testedBefore,
        prevScore: (testedBefore === "نعم") ? prev : "",
        level: document.getElementById("level").value,
        purpose: document.getElementById("purpose").value,
        contactType,
        contactValue,
        notes: document.getElementById("notes").value.trim(),
        receiptName: receipt.name
      };

      const msg = buildMessage(data);
      const url = `https://t.me/${OFFICIAL_USERNAME}?text=${encodeURIComponent(msg)}`;

      tgLink.href = url;
      afterSubmit.classList.remove("hidden");

      // Open Telegram immediately
      window.open(url, "_blank", "noopener");

      showToast("تم تجهيز الرسالة ✅", "افتح تليجرام وأرسل الرسالة ثم أرفق الإيصال مرة ثانية.");
      afterSubmit.scrollIntoView({behavior:"smooth", block:"start"});
    });

    // ====== Toast ======
    const toast = document.getElementById("toast");
    const toastTitle = document.getElementById("toastTitle");
    const toastText = document.getElementById("toastText");
    let toastTimer = null;

    function showToast(title, text){
      toastTitle.textContent = title;
      toastText.textContent = text;
      toast.style.display = "block";
      clearTimeout(toastTimer);
      toastTimer = setTimeout(()=> hideToast(), 6500);
    }
    function hideToast(){
      toast.style.display = "none";
    }

    // ====== Modals ======
    function openModal(id){
      document.getElementById(id).classList.add("active");
    }
    function closeModal(id){
      document.getElementById(id).classList.remove("active");
    }
    window.openModal = openModal;
    window.closeModal = closeModal;

    // ====== Share ======
    function getShareText(){
      return `🚨 دورة STEP المكثفة 2026 (أكاديمية عايد الرسمية)\n\n✅ خطة مختصرة + نماذج حديثة (نموذج 50) + تحديثات 2026 حسب قياس\n💵 السعر الحالي: 299 ريال (بعد الإغلاق 449)\n⏳ التسجيل ينتهي 29/01/2026 أو عند اكتمال العدد\n\nللاشتراك والاستفسار:\n@${OFFICIAL_USERNAME}\nقروب التنبيهات: https://t.me/Academy_Ayed_2026\nبوت مجاني: https://t.me/ayedacadmeybot`;
    }

    function setupShareLinks(){
      const text = encodeURIComponent(getShareText());
      const wa = document.getElementById("shareWa");
      const tg = document.getElementById("shareTg");
      wa.href = `https://wa.me/?text=${text}`;
      tg.href = `https://t.me/share/url?url=${encodeURIComponent(location.href)}&text=${text}`;
    }
    setupShareLinks();

    async function share(){
      const shareData = { title: document.title, text: getShareText(), url: location.href };
      if(navigator.share){
        try{ await navigator.share(shareData); }
        catch(e){}
      }else{
        openModal("shareModal");
      }
    }
    document.getElementById("shareBtn").addEventListener("click", share);
    document.getElementById("shareBtnHero").addEventListener("click", share);
    document.getElementById("shareBtnMobile")?.addEventListener("click", share);

    // ====== Live counters (design/demo) ======
    let req = 17;
    let seats = 62;
    const liveRequests = document.getElementById("liveRequests");
    const seatsLeft = document.getElementById("seatsLeft");

    function bumpCounters(){
      req += Math.random() < .75 ? 1 : 2;
      seats = Math.max(0, seats - (Math.random() < .6 ? 1 : 0));
      liveRequests.textContent = req;
      seatsLeft.textContent = seats;
    }
    setInterval(bumpCounters, 22000);

    // ====== Pop notifications (design/demo) ======
    const names = ["جود","سارة","ريم","نورة","عبدالله","تركي","مايا","ليان","هيا","عمر","شهد","هند"];
    const messages = [
      "قدّم طلب اشتراك جديد",
      "أرسل إيصال التحويل للتأكيد",
      "سأل عن خطة 15 يوم",
      "قال: اختبار قريب واحتاج مكثف",
      "طلب تفعيل سريع",
      "بدأ بخطة المودلز اليوم"
    ];
    function randomItem(arr){ return arr[Math.floor(Math.random()*arr.length)] }
    function popDemoToast(){
      const n = randomItem(names);
      const m = randomItem(messages);
      showToast(`تنبيه: ${n}`, m);
    }
    setInterval(popDemoToast, 45000);
  </script>
</body>
</html>
```0
