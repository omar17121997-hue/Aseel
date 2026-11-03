<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no" />
  <title>اتفاقية الـ100 شيكل مع أسيل ❤️</title>
  
  <!-- Fonts & Confetti -->
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
      --card-bg: rgba(255, 255, 255, 0.94);
      --border-color: rgba(244, 63, 94, 0.2);
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

    /* Floating background icons */
    .bg-icon {
      position: fixed;
      pointer-events: none;
      opacity: 0.18;
      z-index: 0;
      animation: float 6s ease-in-out infinite;
    }

    @keyframes float {
      0%, 100% { transform: translateY(0px) rotate(0deg); }
      50% { transform: translateY(-18px) rotate(8deg); }
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

    /* Header & Progress */
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
      font-size: 1.65rem;
      font-weight: 900;
      background: linear-gradient(135deg, #e11d48 0%, #9333ea 100%);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      margin-bottom: 6px;
      line-height: 1.3;
    }

    .subtitle {
      font-size: 0.9rem;
      color: var(--text-muted);
      margin-bottom: 20px;
      line-height: 1.5;
    }

    /* Progress bar */
    .progress-bar-container {
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 8px;
      margin-bottom: 24px;
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

    /* Pages */
    .step-page {
      display: none;
      animation: fadeIn 0.4s cubic-bezier(0.16, 1, 0.3, 1) forwards;
    }

    .step-page.active {
      display: block;
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(12px); }
      to { opacity: 1; transform: translateY(0); }
    }

    /* Formal Box */
    .formal-box {
      background: #fff;
      border: 1.5px solid #fce7f3;
      border-radius: 24px;
      padding: 22px 18px;
      margin-bottom: 20px;
      text-align: right;
      box-shadow: 0 4px 15px rgba(244, 63, 94, 0.05);
    }

    .formal-box h3 {
      font-size: 1.25rem;
      font-weight: 900;
      color: #be123c;
      margin-bottom: 8px;
      text-align: center;
    }

    .formal-box p {
      font-size: 0.95rem;
      line-height: 1.7;
      color: #334155;
      text-align: center;
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

    /* Options Cards */
    .cards-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 12px;
      margin-bottom: 18px;
    }

    .choice-card {
      background: #ffffff;
      border: 2px solid #f1f5f9;
      border-radius: 22px;
      padding: 18px 12px;
      cursor: pointer;
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 10px;
      transition: all 0.25s ease;
      box-shadow: 0 4px 10px rgba(0,0,0,0.03);
    }

    .choice-card:active {
      transform: scale(0.97);
    }

    .choice-card.selected {
      border-color: #f43f5e;
      background: #fff1f2;
      box-shadow: 0 8px 20px rgba(244, 63, 94, 0.15);
    }

    .card-icon {
      font-size: 32px;
    }

    .card-title {
      font-size: 0.95rem;
      font-weight: 800;
      color: #1e293b;
    }

    /* App terms box */
    .terms-box {
      display: none;
      background: #fdf4ff;
      border: 1.5px solid #f0abfc;
      border-radius: 22px;
      padding: 18px 16px;
      text-align: right;
      margin-top: 16px;
      animation: fadeIn 0.35s ease;
    }

    .terms-box h4 {
      font-size: 0.95rem;
      font-weight: 800;
      color: #86198f;
      margin-bottom: 12px;
    }

    .terms-list {
      list-style: none;
      display: flex;
      flex-direction: column;
      gap: 8px;
    }

    .terms-list li {
      font-size: 0.88rem;
      color: #4a044e;
      display: flex;
      align-items: flex-start;
      gap: 8px;
      line-height: 1.5;
    }

    .terms-list li span.badge-num {
      background: #f5d0fe;
      color: #701a75;
      font-weight: 900;
      width: 22px;
      height: 22px;
      border-radius: 8px;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 0.75rem;
      flex-shrink: 0;
    }

    /* Buttons */
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
      transition: all 0.25s ease;
      box-shadow: 0 8px 20px rgba(0,0,0,0.08);
    }

    .btn:active {
      transform: scale(0.98);
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
      box-shadow: none;
    }

    /* Shopping Check List */
    .shopping-item {
      background: #fff;
      border: 1.5px solid #f1f5f9;
      border-radius: 18px;
      padding: 14px 16px;
      margin-bottom: 10px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      cursor: pointer;
      transition: all 0.2s ease;
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
      width: 24px;
      height: 24px;
      border-radius: 8px;
      border: 2px solid #cbd5e1;
      display: flex;
      align-items: center;
      justify-content: center;
      transition: all 0.2s ease;
      background: #fff;
    }

    .shopping-item.selected .checkbox-box {
      background: #f43f5e;
      border-color: #f43f5e;
      color: #fff;
    }

    /* Custom Suggestion */
    .custom-box {
      background: #fdf4ff;
      border: 1.5px solid #f0abfc;
      border-radius: 18px;
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
      font-family: inherit;
      outline: none;
      margin-top: 10px;
      resize: none;
      background: #fff;
      display: none;
    }

    .custom-textarea:focus {
      border-color: #a855f7;
      box-shadow: 0 0 0 3px rgba(168, 85, 247, 0.15);
    }

    /* Modal (Cash Rejection) */
    .modal-overlay {
      position: fixed;
      inset: 0;
      background: rgba(15, 23, 42, 0.6);
      backdrop-filter: blur(8px);
      display: none;
      align-items: center;
      justify-content: center;
      padding: 20px;
      z-index: 999;
      animation: fadeIn 0.25s ease;
    }

    .modal-content {
      background: #fff;
      border: 3px solid #fda4af;
      border-radius: 28px;
      padding: 26px 20px;
      max-width: 380px;
      width: 100%;
      text-align: center;
      box-shadow: 0 25px 50px -12px rgba(0, 0, 0, 0.25);
    }

    .modal-icon {
      font-size: 48px;
      margin-bottom: 8px;
      animation: shake 0.5s ease;
    }

    @keyframes shake {
      0%, 100% { transform: rotate(0deg); }
      25% { transform: rotate(-10deg); }
      75% { transform: rotate(10deg); }
    }

    /* Final Summary Box */
    .summary-card {
      background: #fff;
      border: 2px dashed #f43f5e;
      border-radius: 24px;
      padding: 20px 18px;
      text-align: right;
      margin-bottom: 20px;
      box-shadow: 0 8px 20px rgba(244, 63, 94, 0.06);
    }

    .summary-row {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 8px 0;
      border-bottom: 1px dashed #f1f5f9;
      font-size: 0.92rem;
    }

    .summary-row:last-child {
      border-bottom: none;
    }

    .summary-row span.label {
      color: #64748b;
      font-weight: 600;
    }

    .summary-row span.val {
      font-weight: 800;
      color: #0f172a;
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
      font-size: 0.8rem;
      font-weight: 700;
    }

    /* Stamp Animation */
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
      animation: stampIn 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    }

    @keyframes stampIn {
      from { transform: scale(2) rotate(-15deg); opacity: 0; }
      to { transform: scale(1) rotate(0deg); opacity: 1; }
    }
  </style>
</head>
<body>

  <!-- Floating decorations -->
  <div class="bg-icon" style="top: 8%; right: 10%; font-size: 26px;">💖</div>
  <div class="bg-icon" style="top: 25%; left: 8%; font-size: 32px; animation-delay: 1.5s;">🛍️</div>
  <div class="bg-icon" style="bottom: 15%; right: 12%; font-size: 30px; animation-delay: 3s;">✨</div>
  <div class="bg-icon" style="bottom: 8%; left: 10%; font-size: 28px; animation-delay: 2s;">🍫</div>

  <div class="container">
    
    <!-- Top Progress & Title -->
    <div class="badge">⚖️ مرسوم مالي رسمي وعاطفي</div>
    <h1 class="main-title">اتفاقية الـ100 شيكل مع أسيل ❤️</h1>
    <p class="subtitle" id="step-indicator">المرحلة الأولى: فحص العرض المالي (1/3)</p>

    <!-- Progress Indicator -->
    <div class="progress-bar-container">
      <div id="prog-1" class="progress-step active"></div>
      <div id="prog-2" class="progress-step"></div>
      <div id="prog-3" class="progress-step"></div>
    </div>

    <!-- ========================================== -->
    <!-- PAGE 1 – THE OFFER -->
    <!-- ========================================== -->
    <div id="page-1" class="step-page active">
      <div class="formal-box">
        <h3>عزيزتنا أسيل ❤️</h3>
        <p>
          بعد التشاور والمداولات، قررنا تقديم عرض مالي بقيمة 
          <span class="budget-tag">100 شيكل</span>، 
          تقديراً إلك وحرصاً على إسعادك.
        </p>
      </div>

      <p style="font-size: 0.9rem; font-weight: 700; color: #475569; margin-bottom: 12px;">
        كيف حابة تستلمي الـ100 شيكل؟ 👇
      </p>

      <div class="cards-grid">
        <!-- 1. Cash -->
        <div class="choice-card" onclick="handleCashClick()">
          <div class="card-icon">💵</div>
          <div class="card-title">نقداً (كاش)</div>
        </div>

        <!-- 2. App -->
        <div class="choice-card" id="app-card" onclick="handleAppClick()">
          <div class="card-icon">📱</div>
          <div class="card-title">عبر التطبيق</div>
        </div>
      </div>

      <!-- App Terms (Appears upon clicking App) -->
      <div id="app-terms" class="terms-box">
        <h4>مسموح، ولكن وفق الشروط والأحكام:</h4>
        <ul class="terms-list">
          <li>
            <span class="badge-num">1</span>
            <span>ممنوع تحويل المبلغ إلى حسابك الشخصي ❌</span>
          </li>
          <li>
            <span class="badge-num">2</span>
            <span>إحنا بنقوم بالشراء عنك مباشرة بكل سرور 🛍️</span>
          </li>
          <li>
            <span class="badge-num">3</span>
            <span>إلك حرية اختيار مشترياتك كاملة كما تحبين ✨</span>
          </li>
          <li>
            <span class="badge-num">4</span>
            <span>الميزانية الإجمالية 100 شيكل فقط لا غير 💰</span>
          </li>
        </ul>

        <button type="button" class="btn btn-primary" style="margin-top: 16px;" onclick="goToPage(2)">
          <span>موافقة والانتقال للاختيارات ❤️</span>
        </button>
      </div>
    </div>

    <!-- ========================================== -->
    <!-- PAGE 2 – SHOPPING OPTIONS -->
    <!-- ========================================== -->
    <div id="page-2" class="step-page">
      <h2 style="font-size: 1.35rem; font-weight: 900; color: #1e293b; margin-bottom: 4px;">
        اختاري مشترياتك يا أسيل 🛍️
      </h2>
      <p style="font-size: 0.88rem; color: #64748b; margin-bottom: 16px;">
        إلك 100 شيكل، اختاري أكثر من خيار حسب رغبتك!
      </p>

      <!-- Options -->
      <div id="shopping-list">
        <div class="shopping-item" onclick="toggleShoppingItem(this, 'شراء كاسة ☕')">
          <div class="item-label">
            <span style="font-size: 1.3rem;">☕</span>
            <span>شراء كاسة</span>
          </div>
          <div class="checkbox-box">✓</div>
        </div>

        <div class="shopping-item" onclick="toggleShoppingItem(this, 'شراء منتوفلي 🍫')">
اتفقنا!</span>
        </button>

        <button type="button" class="btn btn-secondary" style="margin-top: 10px;" onclick="goToPage(2)">
          تعديل الاختيارات
        </button>
      </div>

      <!-- Post-Agreement Celebratory View -->
      <div id="post-celebration" style="display: none;">
        <div class="stamp-c
