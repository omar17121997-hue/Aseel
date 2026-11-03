<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no" />
  <title>اتفاقية الـ100 شيكل مع أسيل ❤️</title>
  
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;600;700;800;900&display=swap" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/canvas-confetti@1.6.0/dist/confetti.browser.min.js"></script>

  <style>
    :root {
      --primary: #f43f5e;
      --primary-dark: #e11d48;
      --accent: #a855f7;
      --bg-gradient: radial-gradient(circle at top center, #fdf2f8 0%, #faf5ff 50%, #fffbeb 100%);
      --card-bg: rgba(255, 255, 255, 0.95);
      --border-color: rgba(244, 63, 94, 0.25);
      --text-main: #1e293b;
      --text-muted: #64748b;
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: 'Cairo', system-ui, -apple-system, sans-serif;
      -webkit-tap-highlight-color: transparent;
      user-select: none;
    }

    body {
      background: var(--bg-gradient);
      color: var(--text-main);
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      padding: 16px;
      overflow-x: hidden;
      position: relative;
    }

    .bg-icon {
      position: fixed;
      pointer-events: none;
      opacity: 0.18;
      z-index: 0;
      animation: float 6s ease-in-out infinite;
    }

    @keyframes float {
      0%, 100% { transform: translateY(0px) rotate(0deg); }
      50% { transform: translateY(-16px) rotate(6deg); }
    }

    .container {
      width: 100%;
      max-width: 480px;
      background: var(--card-bg);
      backdrop-filter: blur(16px);
      -webkit-backdrop-filter: blur(16px);
      border: 1px solid var(--border-color);
      border-radius: 32px;
      padding: 30px 22px;
      box-shadow: 0 20px 45px -10px rgba(244, 63, 94, 0.15), 0 10px 20px -5px rgba(168, 85, 247, 0.1);
      text-align: center;
      position: relative;
      z-index: 10;
    }

    .badge {
      display: inline-flex;
      align-items: center;
      gap: 6px;
      padding: 6px 14px;
      background: #ffe4e6;
      border: 1px solid #fecdd3;
      border-radius: 999px;
      color: #e11d48;
      font-size: 0.82rem;
      font-weight: 700;
      margin-bottom: 12px;
    }

    .main-title {
      font-size: 1.6rem;
      font-weight: 900;
      background: linear-gradient(135deg, #e11d48 0%, #9333ea 100%);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      margin-bottom: 6px;
      line-height: 1.3;
    }

    .subtitle {
      font-size: 0.88rem;
      color: var(--text-muted);
      margin-bottom: 18px;
    }

    .progress-bar-container {
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 8px;
      margin-bottom: 22px;
    }

    .progress-step {
      flex: 1;
      height: 6px;
      background: #f1f5f9;
      border-radius: 999px;
      transition: all 0.4s ease;
    }

    .progress-step.active {
      background: linear-gradient(90deg, #f43f5e, #a855f7);
      box-shadow: 0 0 10px rgba(244, 63, 94, 0.4);
    }

    .progress-step.done {
      background: #10b981;
    }

    .step-page {
      display: none;
      animation: fadeIn 0.35s ease forwards;
    }

    .step-page.active {
      display: block;
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(10px); }
      to { opacity: 1; transform: translateY(0); }
    }

    .formal-box {
      background: #fff;
      border: 1.5px solid #fce7f3;
      border-radius: 24px;
      padding: 22px 18px;
      margin-bottom: 20px;
      text-align: center;
      box-shadow: 0 4px 15px rgba(244, 63, 94, 0.05);
    }

    .formal-box h3 {
      font-size: 1.3rem;
      font-weight: 900;
      color: #be123c;
      margin-bottom: 8px;
    }

    .formal-box p {
      font-size: 0.95rem;
      line-height: 1.7;
      color: #334155;
    }

    .budget-tag {
      display: inline-block;
      background: #fdf2f8;
      border: 1.5px solid #f43f5e;
      color: #e11d48;
      font-weight: 900;
      padding: 2px 10px;
      border-radius: 10px;
      font-size: 1.15rem;
    }

    .cards-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 14px;
      margin-bottom: 10px;
    }

    .choice-card {
      background: #ffffff;
      border: 2.5px solid #e2e8f0;
      border-radius: 24px;
      padding: 22px 12px;
      cursor: pointer;
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 10px;
      transition: all 0.2s ease;
      touch-action: manipulation;
    }

    .choice-card:active {
      transform: scale(0.95);
      border-color: #f43f5e;
      background: #fff1f2;
    }

    .card-icon {
      font-size: 38px;
    }

    .card-title {
      font-size: 1rem;
      font-weight: 800;
      color: #1e293b;
    }

    .btn {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      gap: 8px;
      width: 100%;
      padding: 15px 22px;
      font-size: 1.05rem;
      font-weight: 800;
      border-radius: 20px;
      border: none;
      cursor: pointer;
      text-decoration: none;
      color: #fff;
      transition: all 0.2s ease;
      touch-action: manipulation;
    }

    .btn:active {
      transform: scale(0.97);
    }

    .btn-primary {
      background: linear-gradient(135deg, #f43f5e 0%, #be123c 100%);
      box-shadow: 0 8px 25px rgba(244, 63, 94, 0.35);
    }

    .btn-whatsapp {
      background: linear-gradient(135deg, #22c55e 0%, #16a34a 100%);
      box-shadow: 0 8px 25px rgba(34, 197, 94, 0.35);
      margin-top: 14px;
    }

    .btn-secondary {
      background: #f1f5f9;
      color: #475569;
    }

    /* Shopping Items */
    .shopping-item {
      background: #fff;
      border: 2px solid #f1f5f9;
      border-radius: 20px;
      padding: 14px 16px;
      margin-bottom: 10px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      cursor: pointer;
      transition: all 0.2s ease;
      touch-action: manipulation;
    }

    .shopping-item.selected {
      border-color: #f43f5e;
      background: #fff1f2;
    }

    .item-label {
      display: flex;
      align-items: center;
      gap: 12px;
      font-size: 0.95rem;
      font-weight: 700;
      color: #1e293b;
    }

    .checkbox-box {
      width: 26px;
      height: 26px;
      border-radius: 8px;
      border: 2px solid #cbd5e1;
      display: flex;
      align-items: center;
      justify-content: center;
      background: #fff;
      color: transparent;
      font-weight: 900;
    }

    .shopping-item.selected .checkbox-box {
      background: #f43f5e;
      border-color: #f43f5e;
      color: #fff;
    }

    .custom-box {
      background: #fdf4ff;
      border: 1.5px solid #f0abfc;
      border-radius: 20px;
      padding: 14px 16px;
      margin: 14px 0 20px;
      text-align: right;
    }

    .custom-textarea {
      width: 100%;
      border: 1.5px solid #e9d5ff;
      border-radius: 14px;
      padding: 12px;
      font-size: 0.9rem;
      outline: none;
      margin-top: 10px;
      resize: none;
      background: #fff;
      display: none;
    }

    /* Modals (Popups) */
    .modal-overlay {
      position: fixed;
      inset: 0;
      background: rgba(15, 23, 42, 0.65);
      backdrop-filter: blur(8px);
      display: none;
      align-items: center;
      justify-content: center;
      padding: 20px;
      z-index: 999;
    }

    .modal-content {
      background: #fff;
      border-radius: 28px;
      padding: 26px 20px;
      max-width: 400px;
      width: 100%;
      text-align: center;
      box-shadow: 0 25px 50px -12px rgba(0, 0, 0, 0.3);
      animation: zoomIn 0.25s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    }

    @keyframes zoomIn {
      from { transform: scale(0.9); opacity: 0; }
      to { transform: scale(1); opacity: 1; }
    }

    .summary-card {
      background: #fff;
      border: 2px dashed #f43f5e;
      border-radius: 24px;
      padding: 20px 18px;
      text-align: right;
      margin-bottom: 20px;
    }

    .summary-row {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 8px 0;
      border-bottom: 1px dashed #f1f5f9;
      font-size: 0.92rem;
    }

    .selected-chips {
      display: flex;
      flex-wrap: wrap;
      gap: 6px;
      margin-top: 10px;
    }

    .chip {
      background: #fff1f2;
      border: 1px solid #fecdd3;
      color: #be123c;
      padding: 4px 10px;
      border-radius: 10px;
      font-size: 0.82rem;
      font-weight: 700;
    }

    .stamp-confirmed {
      display: inline-block;
      padding: 6px 16px;
      border: 2px solid #10b981;
      color: #059669;
      border-radius: 14px;
      font-weight: 900;
      font-size: 0.9rem;
      margin-bottom: 16px;
      background: #ecfdf5;
    }
  </style>
</head>
<body>

  <div class="bg-icon" style="top: 8%; right: 10%; font-size: 26px;">💖</div>
  <div class="bg-icon" style="top: 25%; left: 8%; font-size: 32px;">🛍️</div>
  <div class="bg-icon" style="bottom: 15%; right: 12%; font-size: 30px;">✨</div>
  <div class="bg-icon" style="bottom: 8%; left: 10%; font-size: 28px;">🍫</div>

  <div class="container">
    
    <div class="badge">⚖️ مرسوم مالي رسمي وعاطفي</div>
    <h1 class="main-title">اتفاقية الـ100 شيكل مع أسيل ❤️</h1>
    <p class="subtitle" id="step-indicator">المرحلة الأولى: فحص العرض المالي (1/3)</p>

    <!-- Progress Steps -->
    <div class="progress-bar-container">
      <div id="prog-1" class="progress-step active"></div>
      <div id="prog-2" class="progress-step"></div>
      <div id="prog-3" class="progress-step"></div>
    </div>

    <!-- ================= PAGE 1 ================= -->
    <div id="page-1" class="step-page active">
      <div class="formal-box">
        <h3>عزيزتنا أسيل ❤️</h3>
        <p>
          بعد التشاور والمداولات، قررنا تقديم عرض مالي بقيمة 
          <span class="budget-tag">100 شيكل</span>، 
          تقديراً إلك وحرصاً على إسعادك.
        </p>
      </div>

      <p style="font-size: 0.95rem; font-weight: 800; color: #475569; margin-bottom: 14px;">
        اضغطي على طريقة الاستلام المفضلة 👇
      </p>

      <div class="cards-grid">
        <!-- 1. Cash -->
        <div class="choice-card" id="btn-cash" onclick="window.handleCashClick()">
          <div class="card-icon">💵</div>
          <div class="card-title">نقداً (كاش)</div>
        </div>

        <!-- 2. App -->
        <div class="choice-card" id="btn-app" onclick="window.handleAppClick()">
          <div class="card-icon">📱</div>
          <div class="card-title">عبر التطبيق</div>
        </div>
      </div>
    </div>

    <!-- ================= PAGE 2 ================= -->
    <div id="page-2" class="step-page">
      <h2 style="font-size: 1.35rem; font-weight: 900; color: #1e293b; margin-bottom: 4px;">
        اختاري مشترياتك يا أسيل 🛍️
      </h2>
      <p style="font-size: 0.88rem; color: #64748b; margin-bottom: 16px;">
        إلك 100 شيكل، اختاري أكثر من خيار حسب رغبتك!
      </p>

      <div id="shopping-list">
        <div class="shopping-item" onclick="window.toggleShoppingItem(this, 'شراء كاسة ☕')">
          <div class="item-label">
            <span style="font-size: 1.3rem;">☕</span>
            <span>شراء كاسة</span>
          </div>
          <div class="checkbox-box">✓</div>
        </div>

        <div class="shopping-item" onclick="window.toggleShoppingItem(this, 'شراء منتوفلي 🍫')">
          <div class="item-label">
            <span style="font-size: 1.3rem;">🍫</span>
            <span>شراء منتوفلي</span>
          </div>
          <div class="checkbox-box">✓</div>
        </div>

        <div class="shopping-item" onclick="window.toggleShoppingItem(this, 'شراء إكسسوارات 💍')">
          <div class="item-label">
            <span style="font-size: 1.3rem;">💍</span>
            <span>شراء إكسسوارات</span>
          </div>
          <div class="checkbox-box">✓</div>
        </div>

        <div class="shopping-item" onclick="window.toggleShoppingItem(this, 'شراء أسبريه عرق 🥤')">
          <div class="item-label">
            <span style="font-size: 1.3rem;">🥤</span>
            <span>شراء أسبريه عرق</span>
          </div>
          <div class="checkbox-box">✓</div>
        </div>

        <div class="shopping-item" onclick="window.toggleShoppingItem(this, 'مشتريات أخرى 🎁')">
          <div class="item-label">
            <span style="font-size: 1.3rem;">🎁</span>
            <span>مشتريات أخرى</span>
          </div>
          <div class="checkbox-box">✓</div>
        </div>
      </div>

      <!-- Custom Proposal -->
      <div class="custom-box">
        <label style="display: flex; align-items: center; gap: 8px; font-weight: 800; color: #86198f; font-size: 0.9rem; cursor: pointer;">
          <input type="checkbox" id="custom-toggle" onchange="window.toggleCustomArea()" style="accent-color: #a855f7; width: 20px; height: 20px;">
          <span>خيارات أخرى لا تعجبني، عندي اقتراح خاص!</span>
        </label>
        <textarea id="custom-text" class="custom-textarea" rows="3" placeholder="اكتبي شو نفسك نشتريلك..."></textarea>
      </div>

      <div style="display: flex; gap: 10px;">
        <button type="button" class="btn btn-secondary" style="width: 35%;" onclick="window.goToPage(1)">
          رجوع
        </button>
        <button type="button" class="btn btn-primary" style="flex: 1;" onclick="window.goToPage(3)">
          التالي للاتفاق 👈
        </button>
      </div>
    </div>

    <!-- ================= PAGE 3 ================= -->
    <div id="page-3" class="step-page">
      <div id="pre-celebration">
        <h2 style="font-size: 1.4rem; font-weight: 900; color: #1e293b; margin-bottom: 6px;">
          إتمام الاتفاق 🤝❤️
        </h2>
        <p style="font-size: 0.88rem; color: #64748b; margin-bottom: 16px;">
          الملخص النهائي لبنود المعاهدة المالية الرسمية
        </p>

        <div class="summary-card">
          <div class="summary-row">
            <span style="color: #64748b; font-weight: 600;">الميزانية:</span>
            <span style="font-weight: 900; color: #e11d48;">100 شيكل (ILS)</span>
          </div>
          <div class="summary-row">
            <span style="color: #64748b; font-weight: 600;">طريقة الدفع:</span>
            <span style="font-weight: 800;">شراء مباشر منا 🛍️</span>
          </div>
          <div class="summary-row">
            <span style="color: #64748b; font-weight: 600;">التحويل النقدي:</span>
            <span style="font-weight: 800; color: #be123c;">غير مسموح ❌</span>
          </div>

          <div style="margin-top: 10px; font-size: 0.85rem; font-weight: 700; color: #475569;">
            المشتريات المعتمدة لأسيل:
          </div>
          <div class="selected-chips" id="final-items-container"></div>

          <div id="final-custom-container" style="display: none; margin-top: 10px; padding-top: 8px; border-top: 1px dashed #e2e8f0; font-size: 0.88rem; color: #7e22ce;">
            <b>الاقتراح الخاص:</b> <span id="final-custom-text"></span>
          </div>
        </div>

        <div style="background: #fff; border: 2px solid #fecdd3; border-radius: 18px; padding: 14px; margin-bottom: 18px; text-align: right;">
          <label style="display: flex; align-items: center; gap: 10px; font-weight: 800; font-size: 0.95rem; color: #1e293b; cursor: pointer;">
            <input type="checkbox" id="agree-checkbox" onchange="window.toggleAgreeButton()" style="accent-color: #f43f5e; width: 22px; height: 22px;">
            <span>أؤكد موافقتي على الاتفاق.</span>
          </label>
        </div>

        <button type="button" id="agree-final-btn" class="btn btn-primary" style="opacity: 0.5; pointer-events: none;" onclick="window.celebrateAgreement()">
          <span>❤️ اتفقنا!</span>
        </button>

        <button type="button" class="btn btn-secondary" style="margin-top: 10px;" onclick="window.goToPage(2)">
          تعديل الاختيارات
        </button>
      </div>

      <div id="post-celebration" style="display: none;">
        <div class="stamp-confirmed">✓ تم اعتماد الاتفاق رسمياً وبالمحبة</div>
        <div style="font-size: 52px; margin-bottom: 8px;">🎉</div>
        <h2 style="font-size: 1.6rem; font-weight: 900; color: #1e293b; margin-bottom: 8px;">
          مبرووووك يا أسيل! 🎉
        </h2>
        <p style="font-size: 1.05rem; font-weight: 700; color: #059669; line-height: 1.7; margin-bottom: 20px;">
          تم اعتماد طلبك بنجاح!<br>
          استعدي، مشترياتك بالطريق ❤️
        </p>

        <a id="whatsapp-link" href="#" target="_blank" class="btn btn-whatsapp">
          <span>إرسال الاتفاق عبر واتساب 📲</span>
        </a>
      </div>
    </div>

  </div>

  <!-- 1. Cash Rejection Modal -->
  <div id="cash-modal" class="modal-overlay">
    <div class="modal-content" style="border: 3px solid #fda4af;">
      <div style="font-size: 46px; margin-bottom: 6px;">🚫🤣</div>
      <h3 style="font-size: 1.3rem; font-weight: 900; color: #e11d48; margin-bottom: 10px;">
        مرفوض رفضاً قاطعاً! 😂
      </h3>
      <p style="font-size: 0.95rem; line-height: 1.7; color: #334155; margin-bottom: 18px;">
        شو مفكرة الموضوع صراف آلي؟<br>
        <b>النقدي ممنوع منعاً باتاً!</b><br>
        القرار نهائي وغير قابل للاستئناف 🤣
      </p>
      <button type="button" class="btn btn-primary" onclick="window.closeCashModal()">
        فهمت، خلينا ع التطبيق 😅
      </button>
    </div>
  </div>

  <!-- 2. App Terms Approval Modal (Opens directly upon clicking App) -->
  <div id="app-modal" class="modal-overlay">
    <div class="modal-content" style="border: 3px solid #d8b4fe; text-align: right;">
      <div style="text-align: center; font-size: 44px; margin-bottom: 4px;">📱✨</div>
      <h3 style="font-size: 1.25rem; font-weight: 900; color: #7e22ce; margin-bottom: 12px; text-align: center;">
        مسموح، ولكن وفق الشروط والأحكام:
      </h3>
      <div style="background: #faf5ff; border: 1px solid #f3e8ff; border-radius: 16px; padding: 12px; margin-bottom: 18px; font-size: 0.9rem; line-height: 1.8; color: #4a044e;">
        1. ممنوع تحويل المبلغ إلى حسابك الشخصي ❌<br>
        2. إحنا بنقوم بالشراء عنك مباشرة 🛍️<br>
        3. إلك حرية اختيار مشترياتك كاملة ✨<br>
        4. الميزانية الإجمالية 100 شيكل فقط 💰
      </div>
      <button type="button" class="btn btn-primary" onclick="window.confirmTermsAndGo()">
        <span>موافقة والانتقال للاختيارات ❤️</span>
      </button>
    </div>
  </div>

  <script>
    var selectedShopping = [];

    // Global Functions
    window.goToPage = function(pageNum) {
      document.querySelectorAll('.step-page').forEach(function(p) { p.classList.remove('active'); });
      var target = document.getElementById('page-' + pageNum);
      if (target) target.classList.add('active');

      for (var i = 1; i <= 3; i++) {
        var bar = document.getElementById('prog-' + i);
        if (bar) {
          bar.className = 'progress-step';
          if (i < pageNum) bar.classList.add('done');
          if (i === pageNum) bar.classList.add('active');
        }
      }

      var subtitles = {
        1: 'المرحلة الأولى: فحص العرض المالي (1/3)',
        2: 'المرحلة الثانية: تحديد المشتريات (2/3)',
        3: 'المرحلة النهائية: إبرام المعاهدة (3/3)'
      };
      document.getElementById('step-indicator').innerText = subtitles[pageNum] || '';

      if (pageNum === 3) window.renderSummary();
      window.scrollTo({ top: 0, behavior: 'smooth' });
    };

    window.handleCashClick = function() {
      document.getElementById('cash-modal').style.display = 'flex';
    };

    window.closeCashModal = function() {
      document.getElementB
