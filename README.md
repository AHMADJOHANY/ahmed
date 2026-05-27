<html lang="ar" dir="rtl" data-theme="dark"><head>
  <meta charset="UTF-8">
  <title>أحمد سليم الجهني | صفحة شخصية</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <style>
    :root {
      --bg-dark: #020617;
      --bg-dark-elevated: #020617;
      --bg-light: #f9fafb;
      --bg-light-elevated: #ffffff;
      --primary: #2563eb;
      --primary-soft: rgba(37, 99, 235, 0.12);
      --accent: #22d3ee;
      --text-dark: #0f172a;
      --text-light: #e5e7eb;
      --muted-dark: #9ca3af;
      --muted-light: #6b7280;
      --border-dark: #1f2937;
      --border-light: #e5e7eb;
      --radius-lg: 18px;
      --radius-xl: 26px;
      --shadow-soft: 0 18px 45px rgba(15, 23, 42, 0.45);
      --transition-fast: 0.18s ease-out;
      --transition-med: 0.28s ease-out;
    }

    html[data-theme="dark"] {
      --bg: var(--bg-dark);
      --bg-elevated: var(--bg-dark-elevated);
      --text: var(--text-light);
      --muted: var(--muted-dark);
      --border: var(--border-dark);
    }

    html[data-theme="light"] {
      --bg: var(--bg-light);
      --bg-elevated: var(--bg-light-elevated);
      --text: var(--text-dark);
      --muted: var(--muted-light);
      --border: var(--border-light);
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
      background: radial-gradient(circle at top left, #1d4ed8 0, #020617 45%, #020617 100%);
      color: var(--text);
      min-height: 100vh;
      display: flex;
      justify-content: center;
      padding: 24px;
    }

    .shell {
      width: 100%;
      max-width: 1120px;
      background: linear-gradient(135deg, rgba(15, 23, 42, 0.96), rgba(15, 23, 42, 0.98));
      border-radius: 32px;
      padding: 20px;
      position: relative;
      overflow: hidden;
      box-shadow: var(--shadow-soft);
      border: 1px solid rgba(148, 163, 184, 0.25);
    }

    html[data-theme="light"] .shell {
      background: linear-gradient(135deg, #f9fafb, #e5f0ff);
      box-shadow: 0 18px 40px rgba(15, 23, 42, 0.18);
      border-color: rgba(148, 163, 184, 0.45);
    }

    .shell::before {
      content: "";
      position: absolute;
      inset: -40%;
      background:
        radial-gradient(circle at 0% 0%, rgba(56, 189, 248, 0.18), transparent 55%),
        radial-gradient(circle at 100% 0%, rgba(129, 140, 248, 0.18), transparent 55%);
      opacity: 0.9;
      pointer-events: none;
      z-index: -1;
    }

    .shell-inner {
      background: radial-gradient(circle at top, rgba(15, 23, 42, 0.9), rgba(15, 23, 42, 0.98));
      border-radius: 24px;
      padding: 20px 22px 22px;
      border: 1px solid rgba(148, 163, 184, 0.35);
      backdrop-filter: blur(18px);
    }

    html[data-theme="light"] .shell-inner {
      background: rgba(249, 250, 251, 0.9);
      border-color: rgba(148, 163, 184, 0.6);
    }

    header {
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 12px;
      margin-bottom: 18px;
    }

    .brand {
      display: flex;
      align-items: center;
      gap: 10px;
    }

    .brand-logo {
      width: 32px;
      height: 32px;
      border-radius: 999px;
      background: conic-gradient(from 210deg, #22d3ee, #6366f1, #22c55e, #22d3ee);
      padding: 2px;
      position: relative;
      box-shadow: 0 0 0 1px rgba(15, 23, 42, 0.6);
    }

    html[data-theme="light"] .brand-logo {
      box-shadow: 0 0 0 1px rgba(148, 163, 184, 0.7);
    }

    .brand-logo-inner {
      width: 100%;
      height: 100%;
      border-radius: inherit;
      background: radial-gradient(circle at 30% 0%, #e5f0ff, #020617);
      display: flex;
      align-items: center;
      justify-content: center;
      color: #e5f0ff;
      font-weight: 700;
      font-size: 16px;
    }

    .brand-text {
      display: flex;
      flex-direction: column;
      gap: 2px;
    }

    .brand-title {
      font-size: 14px;
      font-weight: 600;
      letter-spacing: 0.03em;
      text-transform: uppercase;
      color: var(--muted);
    }

    .brand-sub {
      font-size: 12px;
      color: var(--muted);
    }

    .controls {
      display: flex;
      align-items: center;
      gap: 8px;
    }

    .chip {
      border-radius: 999px;
      border: 1px solid rgba(148, 163, 184, 0.5);
      padding: 4px 10px;
      font-size: 11px;
      color: var(--muted);
      display: inline-flex;
      align-items: center;
      gap: 6px;
      background: rgba(15, 23, 42, 0.7);
      backdrop-filter: blur(10px);
    }

    html[data-theme="light"] .chip {
      background: rgba(255, 255, 255, 0.9);
    }

    .toggle-btn {
      border-radius: 999px;
      border: 1px solid rgba(148, 163, 184, 0.7);
      padding: 4px 10px;
      font-size: 11px;
      background: rgba(15, 23, 42, 0.9);
      color: var(--text);
      display: inline-flex;
      align-items: center;
      gap: 6px;
      cursor: pointer;
      transition: background var(--transition-fast), transform var(--transition-fast), border-color var(--transition-fast);
    }

    html[data-theme="light"] .toggle-btn {
      background: rgba(255, 255, 255, 0.95);
    }

    .toggle-btn:hover {
      transform: translateY(-1px);
      border-color: var(--primary);
    }

    .toggle-icon {
      width: 16px;
      height: 16px;
      border-radius: 999px;
      background: radial-gradient(circle at 30% 0, #e5f0ff, #1d4ed8);
      display: inline-flex;
      align-items: center;
      justify-content: center;
      color: #e5f0ff;
      font-size: 10px;
    }

    main {
      display: grid;
      grid-template-columns: minmax(0, 1.1fr) minmax(0, 1.1fr);
      gap: 18px;
    }

    @media (max-width: 880px) {
      main {
        grid-template-columns: minmax(0, 1fr);
      }
    }

    .panel {
      background: radial-gradient(circle at top, rgba(15, 23, 42, 0.9), rgba(15, 23, 42, 0.98));
      border-radius: var(--radius-xl);
      padding: 16px 16px 18px;
      border: 1px solid rgba(148, 163, 184, 0.4);
      position: relative;
      overflow: hidden;
    }

    html[data-theme="light"] .panel {
      background: rgba(249, 250, 251, 0.96);
      border-color: rgba(148, 163, 184, 0.7);
    }

    .panel-header {
      display: flex;
      align-items: center;
      justify-content: space-between;
      margin-bottom: 10px;
      gap: 8px;
    }

    .panel-title {
      font-size: 13px;
      font-weight: 600;
      letter-spacing: 0.08em;
      text-transform: uppercase;
      color: var(--muted);
      display: inline-flex;
      align-items: center;
      gap: 6px;
    }

    .pill-dot {
      width: 7px;
      height: 7px;
      border-radius: 999px;
      background: #22d3ee;
      box-shadow: 0 0 0 4px rgba(34, 211, 238, 0.25);
    }

    .panel-badge {
      font-size: 11px;
      color: var(--muted);
    }

    .hero {
      display: grid;
      grid-template-columns: auto minmax(0, 1fr);
      gap: 14px;
      align-items: center;
    }

    @media (max-width: 520px) {
      .hero {
        grid-template-columns: minmax(0, 1fr);
      }
    }

    .avatar-wrap {
      position: relative;
      width: 112px;
      height: 112px;
      border-radius: 32px;
      padding: 3px;
      background: conic-gradient(from 210deg, #22d3ee, #6366f1, #22c55e, #22d3ee);
      box-shadow: 0 18px 40px rgba(15, 23, 42, 0.9);
    }

    html[data-theme="light"] .avatar-wrap {
      box-shadow: 0 18px 32px rgba(15, 23, 42, 0.25);
    }

    .avatar-inner {
      width: 100%;
      height: 100%;
      border-radius: 28px;
      overflow: hidden;
      background: #020617;
      display: flex;
      align-items: center;
      justify-content: center;
    }

    .avatar-inner img {
      width: 100%;
      height: 100%;
      object-fit: cover;
    }

    .avatar-tag {
      position: absolute;
      bottom: -6px;
      inset-inline-start: 10px;
      padding: 4px 8px;
      border-radius: 999px;
      background: rgba(15, 23, 42, 0.9);
      border: 1px solid rgba(148, 163, 184, 0.7);
      font-size: 10px;
      color: var(--muted);
      display: inline-flex;
      align-items: center;
      gap: 4px;
      backdrop-filter: blur(10px);
    }

    html[data-theme="light"] .avatar-tag {
      background: rgba(255, 255, 255, 0.95);
    }

    .hero-text {
      display: flex;
      flex-direction: column;
      gap: 6px;
    }

    .hero-name {
      font-size: 22px;
      font-weight: 700;
      letter-spacing: 0.02em;
    }

    .hero-role {
      font-size: 13px;
      color: var(--muted);
    }

    .hero-highlight {
      margin-top: 4px;
      font-size: 12px;
      color: var(--muted);
    }

    .hero-highlight span {
      color: var(--accent);
      font-weight: 500;
    }

    .hero-actions {
      display: flex;
      flex-wrap: wrap;
      gap: 8px;
      margin-top: 10px;
    }

    .btn {
      border-radius: 999px;
      padding: 7px 14px;
      font-size: 12px;
      border: 1px solid transparent;
      display: inline-flex;
      align-items: center;
      gap: 6px;
      cursor: pointer;
      transition: background var(--transition-med), transform var(--transition-fast), box-shadow var(--transition-fast), border-color var(--transition-fast), color var(--transition-fast);
      text-decoration: none;
    }

    .btn-primary {
      background: linear-gradient(135deg, #2563eb, #4f46e5);
      color: #e5f0ff;
      box-shadow: 0 12px 30px rgba(37, 99, 235, 0.55);
    }

    .btn-primary:hover {
      transform: translateY(-1px);
      box-shadow: 0 16px 40px rgba(37, 99, 235, 0.7);
    }

    .btn-ghost {
      background: rgba(15, 23, 42, 0.7);
      color: var(--muted);
      border-color: rgba(148, 163, 184, 0.7);
    }

    html[data-theme="light"] .btn-ghost {
      background: rgba(255, 255, 255, 0.9);
    }

    .btn-ghost:hover {
      border-color: var(--primary);
      color: var(--text);
      transform: translateY(-1px);
    }

    .hero-meta {
      display: flex;
      flex-wrap: wrap;
      gap: 6px;
      margin-top: 10px;
      font-size: 11px;
      color: var(--muted);
    }

    .hero-meta span {
      padding: 4px 8px;
      border-radius: 999px;
      background: rgba(15, 23, 42, 0.7);
      border: 1px solid rgba(148, 163, 184, 0.6);
    }

    html[data-theme="light"] .hero-meta span {
      background: rgba(255, 255, 255, 0.9);
    }

    .section {
      margin-top: 10px;
    }

    .section-title {
      font-size: 12px;
      text-transform: uppercase;
      letter-spacing: 0.12em;
      color: var(--muted);
      margin-bottom: 8px;
      display: flex;
      align-items: center;
      gap: 6px;
    }

    .section-title::before {
      content: "";
      width: 18px;
      height: 1px;
      background: linear-gradient(to left, rgba(148, 163, 184, 0), rgba(148, 163, 184, 0.9));
    }

    .section-body {
      font-size: 13px;
      color: var(--muted);
      line-height: 1.7;
    }

    .grid-two {
      display: grid;
      grid-template-columns: minmax(0, 1fr) minmax(0, 1fr);
      gap: 10px;
      margin-top: 6px;
    }

    @media (max-width: 640px) {
      .grid-two {
        grid-template-columns: minmax(0, 1fr);
      }
    }

    .pill-list {
      display: flex;
      flex-wrap: wrap;
      gap: 6px;
      margin-top: 6px;
    }

    .pill {
      font-size: 11px;
      padding: 5px 9px;
      border-radius: 999px;
      background: rgba(15, 23, 42, 0.7);
      border: 1px solid rgba(148, 163, 184, 0.6);
      color: var(--muted);
    }

    html[data-theme="light"] .pill {
      background: rgba(255, 255, 255, 0.9);
    }

    .timeline {
      margin-top: 6px;
      display: flex;
      flex-direction: column;
      gap: 8px;
    }

    .timeline-item {
      display: grid;
      grid-template-columns: auto minmax(0, 1fr);
      gap: 8px;
      align-items: flex-start;
    }

    .timeline-marker {
      width: 9px;
      height: 9px;
      border-radius: 999px;
      background: #22d3ee;
      margin-top: 5px;
      box-shadow: 0 0 0 4px rgba(34, 211, 238, 0.25);
    }

    .timeline-content {
      border-radius: 14px;
      padding: 7px 9px;
      background: rgba(15, 23, 42, 0.7);
      border: 1px solid rgba(148, 163, 184, 0.5);
      font-size: 12px;
      color: var(--muted);
    }

    html[data-theme="light"] .timeline-content {
      background: rgba(255, 255, 255, 0.95);
    }

    .timeline-title {
      font-weight: 600;
      color: var(--text);
      margin-bottom: 2px;
      font-size: 12px;
    }

    .timeline-sub {
      font-size: 11px;
      margin-bottom: 2px;
    }

    .timeline-meta {
      font-size: 11px;
      opacity: 0.9;
    }

    .tag-row {
      display: flex;
      flex-wrap: wrap;
      gap: 6px;
      margin-top: 4px;
    }

    .tag {
      font-size: 10px;
      padding: 3px 7px;
      border-radius: 999px;
      background: rgba(15, 23, 42, 0.8);
      border: 1px solid rgba(148, 163, 184, 0.6);
      color: var(--muted);
    }

    html[data-theme="light"] .tag {
      background: rgba(255, 255, 255, 0.95);
    }

    .contact-card {
      margin-top: 8px;
      border-radius: 16px;
      padding: 10px 11px;
      background: rgba(15, 23, 42, 0.85);
      border: 1px solid rgba(148, 163, 184, 0.6);
      font-size: 12px;
      color: var(--muted);
      display: grid;
      grid-template-columns: minmax(0, 1.2fr) minmax(0, 1fr);
      gap: 8px;
      align-items: center;
    }

    html[data-theme="light"] .contact-card {
      background: rgba(255, 255, 255, 0.96);
    }

    @media (max-width: 640px) {
      .contact-card {
        grid-template-columns: minmax(0, 1fr);
      }
    }

    .contact-main {
      display: flex;
      flex-direction: column;
      gap: 3px;
    }

    .contact-main strong {
      color: var(--text);
      font-size: 12px;
    }

    .contact-actions {
      display: flex;
      flex-wrap: wrap;
      gap: 6px;
      justify-content: flex-end;
    }

    @media (max-width: 640px) {
      .contact-actions {
        justify-content: flex-start;
      }
    }

    .file-input {
      margin-top: 6px;
      font-size: 11px;
      color: var(--muted);
      display: flex;
      flex-direction: column;
      gap: 4px;
    }

    .file-input input[type="file"] {
      font-size: 11px;
      color: var(--muted);
    }

    .badge-row {
      display: flex;
      flex-wrap: wrap;
      gap: 6px;
      margin-top: 6px;
      font-size: 10px;
      color: var(--muted);
    }

    .badge-soft {
      padding: 4px 8px;
      border-radius: 999px;
      background: rgba(37, 99, 235, 0.12);
      border: 1px solid rgba(37, 99, 235, 0.4);
      color: #bfdbfe;
    }

    html[data-theme="light"] .badge-soft {
      background: rgba(37, 99, 235, 0.08);
      color: #1d4ed8;
    }

    .badge-soft span {
      opacity: 0.8;
    }

    .fade-in {
      opacity: 0;
      transform: translateY(8px);
      animation: fadeInUp 0.6s var(--transition-med) forwards;
    }

    .fade-in.delay-1 {
      animation-delay: 0.08s;
    }

    .fade-in.delay-2 {
      animation-delay: 0.16s;
    }

    .fade-in.delay-3 {
      animation-delay: 0.24s;
    }

    @keyframes fadeInUp {
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }
  </style>
</head>
<body>
  <div class="shell">
    <div class="shell-inner">
      <header>
        <div class="brand">
          
          <div class="brand-text">
            <div class="brand-title" data-i18n="brandTitle">سيرتي الذاتية</div>
            <div class="brand-sub" data-i18n="brandSub">تم تصميم هذه الصفحة باستخدام نموذج Smart من  Copilot</div>
          </div>
        </div>
        <div class="controls">
          <div class="chip">
            <span style="width:7px;height:7px;border-radius:999px;background:#22c55e;"></span>
            <span data-i18n="status">متاح للتعاون</span>
          </div>
          <button class="toggle-btn" id="langToggle">
            <span class="toggle-icon">🌐</span>
            <span id="langLabel">العربية / EN</span>
          </button>
          <button class="toggle-btn" id="themeToggle">
            <span class="toggle-icon">☾</span>
            <span data-i18n="themeLabel">الوضع الداكن</span>
          </button>
        </div>
      </header>

      <main>
        <!-- اللوحة اليسرى: البطل + الملخص + المهارات -->
        <section class="panel fade-in">
          <div class="panel-header">
            <div class="panel-title">
              <span class="pill-dot"></span>
              <span data-i18n="heroPanelTitle">نظرة عامة</span>
            </div>
            <div class="panel-badge" data-i18n="heroPanelBadge">خدمة عملاء ومهارات بيانات</div>
          </div>

          <div class="hero">
            <div>
              
              
            </div>

            <div class="hero-text">
              <div class="hero-name" data-i18n="name">أحمد سليم حسن الجهني</div>
              <div class="hero-role" data-i18n="role">مساعد خدمات عملاء | خبير خدمة عملاء وبيانات</div>
              <div class="hero-highlight" data-i18n="heroHighlight">يعمل حالياً في <span>الشركة السعودية للكهرباء</span> منذ 2011 مع خبرة سابقة في قطاع الفنادق.</div>

              

              <div class="hero-meta">
                <span data-i18n="metaLocation">المدينة المنورة، المملكة العربية السعودية</span>
                <span data-i18n="metaExperience">خبرة منذ 2005</span>
                <span data-i18n="metaLanguages">العربية، الإنجليزية B1</span>
              </div>
            </div>
          </div>

          <div class="section">
            <div class="section-title" data-i18n="aboutTitle">نبذة</div>
            <div class="section-body" data-i18n="aboutBody">محترف في خدمة العملاء وإدارة المكاتب مع خبرة تمتد من قطاع الضيافة (فنادق إيلاف) إلى قطاع الطاقة (الشركة السعودية للكهرباء)، يجمع بين المهارات الإدارية والقدرة على التعامل مع الأنظمة المتقدمة والبيانات، مع اهتمام خاص بتطوير لوحات معلومات تفاعلية وتحسين تجربة العميل.</div>
          </div>

          <div class="section">
            <div class="section-title" data-i18n="skillsTitle">أهم المهارات</div>
            <div class="grid-two">
              <div>
                <div class="section-body" data-i18n="skillsTechTitle" style="font-weight:600;font-size:12px;margin-bottom:4px;">مهارات تقنية</div>
                <div class="pill-list">
                  <span class="pill" data-i18n="skillOffice">Microsoft Office (متقدم)</span>
                  <span class="pill" data-i18n="skillPowerBI">Microsoft Power BI (لوحات تفاعلية)</span>
                  <span class="pill" data-i18n="skillProject">Microsoft Project</span>
                  <span class="pill" data-i18n="skillBigData">التعامل مع البيانات الضخمة</span>
                  <span class="pill" data-i18n="skillHTMLCSS">أساسيات HTML &amp; CSS</span>
                  <span class="pill" data-i18n="skillAI">أدوات الذكاء الاصطناعي (ChatGPT, Claude, Google AI Studio)</span>
                </div>
              </div>
              <div>
                <div class="section-body" data-i18n="skillsSoftTitle" style="font-weight:600;font-size:12px;margin-bottom:4px;">مهارات شخصية وإدارية</div>
                <div class="pill-list">
                  <span class="pill" data-i18n="skillOfficeMgmt">إدارة المكاتب وتنظيم العمل</span>
                  <span class="pill" data-i18n="skillTeam">تكوين فريق عمل محترف</span>
                  <span class="pill" data-i18n="skillComm">اللباقة وحسن الإنصات</span>
                  <span class="pill" data-i18n="skillEQ">الذكاء العاطفي</span>
                  <span class="pill" data-i18n="skillNegotiation">التفاوض الفعال</span>
                  <span class="pill" data-i18n="skillStress">إدارة ضغوط العمل</span>
                </div>
              </div>
            </div>
          </div>

          <div class="section">
            <div class="section-title" data-i18n="systemsTitle">الأنظمة التي عملت عليها</div>
            <div class="pill-list">
              <span class="pill">SAP (Billing, Time, ESS, TPS)</span>
              <span class="pill">CRM</span>
              <span class="pill">UDIS</span>
              <span class="pill">Mainframe Billing</span>
              <span class="pill">Fidelio / Opera / Micros</span>
              <span class="pill">Microsoft SharePoint</span>
              <span class="pill">GIS (Query)</span>
            </div>
          </div>
        </section>

        <!-- اللوحة اليمنى: الخبرة + الدورات + التواصل -->
        <section class="panel fade-in delay-1">
          <div class="panel-header">
            <div class="panel-title">
              <span class="pill-dot"></span>
              <span data-i18n="expPanelTitle">الخبرة والنمو المهني</span>
            </div>
            <div class="panel-badge" data-i18n="expPanelBadge">من الضيافة إلى قطاع الطاقة</div>
          </div>

          <div class="section">
            <div class="section-title" data-i18n="experienceTitle">مسار الخبرة</div>
            <div class="timeline">
              <div class="timeline-item">
                <div class="timeline-marker"></div>
                <div class="timeline-content">
                  <div class="timeline-title" data-i18n="expSECNowTitle">مساعد خدمات عملاء – مكتب كهرباء المدينة</div>
                  <div class="timeline-sub" data-i18n="expSECNowSub">الشركة السعودية للكهرباء | من 2 مايو 2024 حتى الآن</div>
                  <div class="timeline-meta" data-i18n="expSECNowMeta">دعم العملاء، إدارة الطلبات، التعامل مع أنظمة الفوترة والعدادات الذكية، وتحسين تجربة المستفيد.</div>
                  <div class="tag-row">
                    <span class="tag" data-i18n="tagSmartMeters">العدادات الذكية</span>
                    <span class="tag" data-i18n="tagCRM">نظام CRM</span>
                    <span class="tag" data-i18n="tagSAP">SAP ISU Billing</span>
                  </div>
                </div>
              </div>

              <div class="timeline-item">
                <div class="timeline-marker"></div>
                <div class="timeline-content">
                  <div class="timeline-title" data-i18n="expSECPrevTitle">كاتب خدمات عملاء – مكاتب كهرباء الخبر والمدينة</div>
                  <div class="timeline-sub" data-i18n="expSECPrevSub">الشركة السعودية للكهرباء | 2012 – 2024</div>
                  <div class="timeline-meta" data-i18n="expSECPrevMeta">استقبال ومعالجة طلبات العملاء، متابعة الفوترة، استخدام أنظمة التوزيع الموحد، والمشاركة في تحسين جودة الخدمة.</div>
                  <div class="tag-row">
                    <span class="tag">UDIS</span>
                    <span class="tag">Mainframe</span>
                    <span class="tag">SharePoint</span>
                  </div>
                </div>
              </div>

              <div class="timeline-item">
                <div class="timeline-marker"></div>
                <div class="timeline-content">
                  <div class="timeline-title" data-i18n="expElafTitle">كبير محاسبين / مشرف حسابات – فنادق إيلاف</div>
                  <div class="timeline-sub" data-i18n="expElafSub">مجموعة إيلاف للفنادق | 2005 – 2011</div>
                  <div class="timeline-meta" data-i18n="expElafMeta">مراجعة الدخل والإيرادات، الإشراف على الحسابات، التعامل مع أنظمة إدارة الفنادق والمطاعم، وضبط التقارير المالية.</div>
                  <div class="tag-row">
                    <span class="tag">Fidelio</span>
                    <span class="tag">Opera</span>
                    <span class="tag">Micros</span>
                    <span class="tag">Oracle GL</span>
                  </div>
                </div>
              </div>
            </div>
          </div>

          <div class="section">
            <div class="section-title" data-i18n="coursesTitle">دورات مختارة</div>
            <div class="badge-row">
              <span class="badge-soft" data-i18n="courseCustomerCare">خدمة العملاء والتميز في العناية بالعميل</span>
              <span class="badge-soft" data-i18n="courseInfographic">تصميم الإنفوجرافيك</span>
              <span class="badge-soft" data-i18n="courseProject">Microsoft Project 2013</span>
              <span class="badge-soft" data-i18n="courseCRM">نظام إدارة علاقات العملاء CRM</span>
              <span class="badge-soft" data-i18n="courseSafety">السلامة، الإطفاء، السياقة الوقائية</span>
              <span class="badge-soft" data-i18n="courseFirstAid">الإسعافات الأولية</span>
            </div>
          </div>

          <div class="section">
            <div class="section-title" data-i18n="volunteerTitle">الأعمال التطوعية</div>
            <div class="section-body" data-i18n="volunteerBody">عضو داعم تقني في مجلس حي الفتح بالمدينة المنورة منذ يونيو 2023، مع مساهمة في دعم الأنشطة المجتمعية وتنظيم العمل التقني.</div>
          </div>

          <div class="section" id="contact">
            <div class="section-title" data-i18n="contactTitle">التواصل</div>
            <div class="contact-card">
              <div class="contact-main">
                <strong data-i18n="contactLine">جاهز للتعاون في مشاريع خدمة العملاء، البيانات، ولوحات المعلومات.</strong>
                <div>
                  <span data-i18n="contactPhoneLabel">الجوال:</span>
                  <span dir="ltr">+966556693651</span>
                </div>
                <div>
                  <span data-i18n="contactEmailLabel">البريد الإلكتروني:</span>
                  <a href="mailto:ahmedjohany@gmail.com" style="color:var(--accent);text-decoration:none;">
                    ahmedjohany@gmail.com
                  </a>
                </div>
              </div>
              <div class="contact-actions">
                <a href="tel:+966556693651" class="btn btn-primary" data-i18n="contactCall">اتصال مباشر</a>
                <a href="mailto:ahmedjohany@gmail.com" class="btn btn-ghost" data-i18n="contactMail">إرسال بريد</a>
              </div>
            </div>
          </div>
        </section>
      </main>
    </div>
  </div>

  <script>
    const translations = {
      ar: {
        brandTitle: "سيرتي الذاتية وحياتي العملية",
        brandSub: "تم تصميم هذه الصفحة باستخدام نموذج Smart من  Copilot",
        status: "متاح للتعاون",
        themeLabel: "الوضع الداكن",
        heroPanelTitle: "نظرة عامة",
        heroPanelBadge: "خدمة عملاء ومهارات بيانات",
        avatarTag: "+19 سنة خبرة",
        photoLabel: "رفع صورة شخصية (لن تُرفع للإنترنت، محلي فقط)",
        name: "أحمد سليم حسن الجهني",
        role: "مساعد خدمات عملاء | خبير خدمة عملاء وبيانات",
        heroHighlight:
          "يعمل حالياً في <span>الشركة السعودية للكهرباء</span> منذ 2011 مع خبرة سابقة في قطاع الفنادق.",
        btnPrimary: "تحميل السيرة الذاتية PDF",
        btnSecondary: "تواصل معي",
        metaLocation: "المدينة المنورة، المملكة العربية السعودية",
        metaExperience: "خبرة منذ 2005",
        metaLanguages: "العربية، الإنجليزية B1",
        aboutTitle: "نبذة",
        aboutBody:
          "محترف في خدمة العملاء وإدارة المكاتب مع خبرة تمتد من قطاع الضيافة (فنادق إيلاف) إلى قطاع الطاقة (الشركة السعودية للكهرباء)، يجمع بين المهارات الإدارية والقدرة على التعامل مع الأنظمة المتقدمة والبيانات، مع اهتمام خاص بتطوير لوحات معلومات تفاعلية وتحسين تجربة العميل.",
        skillsTitle: "أهم المهارات",
        skillsTechTitle: "مهارات تقنية",
        skillsSoftTitle: "مهارات شخصية وإدارية",
        skillOffice: "Microsoft Office (متقدم)",
        skillPowerBI: "Microsoft Power BI (لوحات تفاعلية)",
        skillProject: "Microsoft Project",
        skillBigData: "التعامل مع البيانات الضخمة",
        skillHTMLCSS: "أساسيات HTML & CSS",
        skillAI: "أدوات الذكاء الاصطناعي (ChatGPT, Claude, Google AI Studio)",
        skillOfficeMgmt: "إدارة المكاتب وتنظيم العمل",
        skillTeam: "تكوين فريق عمل محترف",
        skillComm: "اللباقة وحسن الإنصات",
        skillEQ: "الذكاء العاطفي",
        skillNegotiation: "التفاوض الفعال",
        skillStress: "إدارة ضغوط العمل",
        systemsTitle: "الأنظمة التي عملت عليها",
        expPanelTitle: "الخبرة والنمو المهني",
        expPanelBadge: "من الضيافة إلى قطاع الطاقة",
        experienceTitle: "مسار الخبرة",
        expSECNowTitle: "مساعد خدمات عملاء – مكتب كهرباء المدينة",
        expSECNowSub: "الشركة السعودية للكهرباء | من 2 مايو 2024 حتى الآن",
        expSECNowMeta:
          "دعم العملاء، إدارة الطلبات، التعامل مع أنظمة الفوترة والعدادات الذكية، وتحسين تجربة المستفيد.",
        tagSmartMeters: "العدادات الذكية",
        tagCRM: "نظام CRM",
        tagSAP: "SAP ISU Billing",
        expSECPrevTitle: "كاتب خدمات عملاء – مكاتب كهرباء الخبر والمدينة",
        expSECPrevSub: "الشركة السعودية للكهرباء | 2012 – 2024",
        expSECPrevMeta:
          "استقبال ومعالجة طلبات العملاء، متابعة الفوترة، استخدام أنظمة التوزيع الموحد، والمشاركة في تحسين جودة الخدمة.",
        expElafTitle: "كبير محاسبين / مشرف حسابات – فنادق إيلاف",
        expElafSub: "مجموعة إيلاف للفنادق | 2005 – 2011",
        expElafMeta:
          "مراجعة الدخل والإيرادات، الإشراف على الحسابات، التعامل مع أنظمة إدارة الفنادق والمطاعم، وضبط التقارير المالية.",
        coursesTitle: "دورات مختارة",
        courseCustomerCare: "خدمة العملاء والتميز في العناية بالعميل",
        courseInfographic: "تصميم الإنفوجرافيك",
        courseProject: "Microsoft Project 2013",
        courseCRM: "نظام إدارة علاقات العملاء CRM",
        courseSafety: "السلامة، الإطفاء، السياقة الوقائية",
        courseFirstAid: "الإسعافات الأولية",
        volunteerTitle: "الأعمال التطوعية",
        volunteerBody:
          "عضو داعم تقني في مجلس حي الفتح بالمدينة المنورة منذ يونيو 2023، مع مساهمة في دعم الأنشطة المجتمعية وتنظيم العمل التقني.",
        contactTitle: "التواصل",
        contactLine:
          "جاهز للتعاون في مشاريع خدمة العملاء، البيانات، ولوحات المعلومات.",
        contactPhoneLabel: "الجوال:",
        contactEmailLabel: "البريد الإلكتروني:",
        contactCall: "اتصال مباشر",
        contactMail: "إرسال بريد"
      },
      en: {
        brandTitle: "Curriculum Vitae",
        brandSub: "This page was created utilizing the Smart design model provided by Copilot.",
        status: "Available for collaboration",
        themeLabel: "Dark",
        heroPanelTitle: "Overview",
        heroPanelBadge: "Customer Service & Data Skills",
        avatarTag: "+19 yrs experience",
        photoLabel: "Upload profile photo (local only, not uploaded)",
        name: "Ahmed Saleem Hassan Al-Juhani",
        role: "Customer Service Assistant | Customer Care & Data",
        heroHighlight:
          "Currently working at <span>Saudi Electricity Company</span> since 2011, with prior experience in the hospitality sector.",
        btnPrimary: "Download CV (PDF)",
        btnSecondary: "Contact me",
        metaLocation: "Al-Madinah Al-Munawwarah, Saudi Arabia",
        metaExperience: "Experience since 2005",
        metaLanguages: "Arabic, English B1",
        aboutTitle: "About",
        aboutBody:
          "A customer service and office management professional with experience spanning hospitality (Elaf Hotels) and the energy sector (Saudi Electricity Company), combining administrative skills with strong systems and data handling, with a focus on interactive dashboards and customer experience.",
        skillsTitle: "Key Skills",
        skillsTechTitle: "Technical Skills",
        skillsSoftTitle: "Soft & Administrative Skills",
        skillOffice: "Microsoft Office (Advanced)",
        skillPowerBI: "Microsoft Power BI (Interactive dashboards)",
        skillProject: "Microsoft Project",
        skillBigData: "Big data handling",
        skillHTMLCSS: "Basic HTML & CSS",
        skillAI: "AI tools (ChatGPT, Claude, Google AI Studio)",
        skillOfficeMgmt: "Office management & workflow",
        skillTeam: "Building professional teams",
        skillComm: "Communication & active listening",
        skillEQ: "Emotional intelligence",
        skillNegotiation: "Effective negotiation",
        skillStress: "Work stress management",
        systemsTitle: "Systems Experience",
        expPanelTitle: "Experience & Growth",
        expPanelBadge: "Hotels → Energy Sector",
        experienceTitle: "Experience Timeline",
        expSECNowTitle: "Customer Service Assistant – Medina Office",
        expSECNowSub: "Saudi Electricity Company | May 2, 2024 – Present",
        expSECNowMeta:
          "Supporting customers, managing requests, working with billing and smart meter systems, and enhancing customer experience.",
        tagSmartMeters: "Smart meters",
        tagCRM: "CRM system",
        tagSAP: "SAP ISU Billing",
        expSECPrevTitle: "Customer Service Clerk – Khobar & Medina Offices",
        expSECPrevSub: "Saudi Electricity Company | 2012 – 2024",
        expSECPrevMeta:
          "Handling customer requests, billing follow-up, using unified distribution systems, and contributing to service quality.",
        expElafTitle: "Senior Accountant / Accounts Supervisor – Elaf Hotels",
        expElafSub: "Elaf Hotels Group | 2005 – 2011",
        expElafMeta:
          "Reviewing revenue, supervising accounts, working with hotel and restaurant management systems, and preparing financial reports.",
        coursesTitle: "Selected Courses",
        courseCustomerCare: "Customer Care & Service Excellence",
        courseInfographic: "Infographic Design",
        courseProject: "Microsoft Project 2013",
        courseCRM: "Customer Relationship Management (CRM)",
        courseSafety: "Safety, Firefighting, Defensive Driving",
        courseFirstAid: "First Aid",
        volunteerTitle: "Volunteer Work",
        volunteerBody:
          "Technical support member at Al-Fath District Council in Medina since June 2023, contributing to community activities and technical organization.",
        contactTitle: "Contact",
        contactLine:
          "Open to collaboration on customer service, data, and dashboard projects.",
        contactPhoneLabel: "Mobile:",
        contactEmailLabel: "Email:",
        contactCall: "Call now",
        contactMail: "Send email"
      }
    };

    let currentLang = "ar";

    function applyTranslations() {
      const dict = translations[currentLang];
      document.documentElement.lang = currentLang;
      document.documentElement.dir = currentLang === "ar" ? "rtl" : "ltr";

      document.querySelectorAll("[data-i18n]").forEach((el) => {
        const key = el.getAttribute("data-i18n");
        if (!dict[key]) return;
        if (dict[key].includes("<span")) {
          el.innerHTML = dict[key];
        } else {
          el.textContent = dict[key];
        }
      });

      const langLabel = document.getElementById("langLabel");
      langLabel.textContent = currentLang === "ar" ? "العربية / EN" : "English / AR";
    }

    document.getElementById("langToggle").addEventListener("click", () => {
      currentLang = currentLang === "ar" ? "en" : "ar";
      applyTranslations();
    });

    const themeToggle = document.getElementById("themeToggle");
    function setTheme(theme) {
      document.documentElement.setAttribute("data-theme", theme);
      const label = themeToggle.querySelector("[data-i18n='themeLabel']");
      if (label) {
        label.textContent = theme === "dark" ? (currentLang === "ar" ? "الوضع الداكن" : "Dark") : (currentLang === "ar" ? "الوضع الفاتح" : "Light");
      }
      const icon = themeToggle.querySelector(".toggle-icon");
      if (icon) {
        icon.textContent = theme === "dark" ? "☾" : "☀";
      }
    }

    themeToggle.addEventListener("click", () => {
      const current = document.documentElement.getAttribute("data-theme") || "dark";
      setTheme(current === "dark" ? "light" : "dark");
    });

    const prefersDark = window.matchMedia && window.matchMedia("(prefers-color-scheme: dark)").matches;
    setTheme(prefersDark ? "dark" : "light");
    applyTranslations();

    const photoInput = document.getElementById("photoUpload");
    const photoImg = document.getElementById("profilePhoto");

    photoInput.addEventListener("change", (e) => {
      const file = e.target.files[0];
      if (!file) return;
      const reader = new FileReader();
      reader.onload = (ev) => {
        photoImg.src = ev.target.result;
      };
      reader.readAsDataURL(file);
    });
  </script>


</body></html>
