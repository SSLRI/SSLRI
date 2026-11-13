```html
<!DOCTYPE html>
<html lang="fa" dir="rtl" class="dark">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>GitHub Profile & README Preview - SSLRI</title>
  <!-- Tailwind CSS -->
  <script src="https://cdn.tailwindcss.com"></script>
  <!-- Google Fonts: Vazirmatn (Persian UI), Inter (GitHub UI), Fira Code (Typing SVG) -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Fira+Code:wght@500;600;700&family=Inter:wght@400;500;600;700&family=Vazirmatn:wght@400;500;600;700&display=swap" rel="stylesheet">
  
  <style>
    :root {
      --gh-bg: #0d1117;
      --gh-card: #161b22;
      --gh-border: #30363d;
      --gh-text: #c9d1d9;
      --gh-muted: #8b949e;
      --gh-link: #58a6ff;
      --gh-btn: #21262d;
      --gh-btn-hover: #30363d;
    }

    body {
      background-color: var(--gh-bg);
      color: var(--gh-text);
      font-family: 'Vazirmatn', sans-serif;
      overflow-x: hidden;
    }

    /* GitHub Authentic LTR Container */
    .gh-ltr {
      direction: ltr;
      text-align: left;
      font-family: -apple-system, BlinkMacSystemFont, 'Inter', 'Segoe UI', Helvetica, Arial, sans-serif;
    }

    .font-fira {
      font-family: 'Fira Code', monospace;
    }

    /* Typing Cursor Animation */
    .typing-cursor {
      display: inline-block;
      width: 3px;
      height: 1.2em;
      vertical-align: middle;
      margin-left: 4px;
      animation: blink 0.85s infinite;
    }

    @keyframes blink {
      0%, 100% { opacity: 1; }
      50% { opacity: 0; }
    }

    /* Animated Dev Illustration Keyframes */
    @keyframes floatSlow {
      0%, 100% { transform: translateY(0px); }
      50% { transform: translateY(-6px); }
    }
    @keyframes pulseGlow {
      0%, 100% { opacity: 0.5; }
      50% { opacity: 1; }
    }
    @keyframes codeScroll {
      0% { transform: translateY(0); }
      50% { transform: translateY(-8px); }
      100% { transform: translateY(0); }
    }

    .dev-float {
      animation: floatSlow 4s ease-in-out infinite;
    }
    .glow-pulse {
      animation: pulseGlow 2.5s ease-in-out infinite;
    }
    .code-anim {
      animation: codeScroll 3s ease-in-out infinite;
    }

    /* Custom Scrollbar */
    ::-webkit-scrollbar {
      width: 8px;
      height: 8px;
    }
    ::-webkit-scrollbar-track {
      background: #0d1117;
    }
    ::-webkit-scrollbar-thumb {
      background: #30363d;
      border-radius: 4px;
    }
    ::-webkit-scrollbar-thumb:hover {
      background: #484f58;
    }

    /* Mobile Frame Simulation */
    .mobile-frame {
      max-width: 412px;
      margin: 0 auto;
      border: 8px solid #21262d;
      border-radius: 32px;
      box-shadow: 0 25px 50px -12px rgba(0, 0, 0, 0.75), 0 0 0 1px #30363d;
      overflow: hidden;
      background-color: #0d1117;
      transition: all 0.35s cubic-bezier(0.4, 0, 0.2, 1);
    }

    .desktop-frame {
      max-width: 1240px;
      margin: 0 auto;
      transition: all 0.35s cubic-bezier(0.4, 0, 0.2, 1);
    }
  </style>
</head>
<body class="min-h-screen flex flex-col">

  <!-- ================= TOP PERSIAN CONTROL TOOLBAR ================= -->
  <header class="sticky top-0 z-50 bg-[#161b22]/95 backdrop-blur-md border-b border-[#30363d] px-4 py-3 shadow-lg">
    <div class="max-w-7xl mx-auto flex flex-wrap items-center justify-between gap-3">
      
      <!-- Brand / Title -->
      <div class="flex items-center gap-2.5">
        <div class="w-9 h-9 rounded-xl bg-cyan-500/10 border border-cyan-500/30 flex items-center justify-center text-cyan-400">
          <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24">
            <path fill-rule="evenodd" clip-rule="evenodd" d="M12 2C6.477 2 2 6.484 2 12.017c0 4.425 2.865 8.18 6.839 9.504.5.092.682-.217.682-.483 0-.237-.008-.868-.013-1.703-2.782.605-3.369-1.343-3.369-1.343-.454-1.158-1.11-1.466-1.11-1.466-.908-.62.069-.608.069-.608 1.003.07 1.53 1.032 1.53 1.032.892 1.53 2.341 1.088 2.91.832.092-.647.35-1.088.636-1.338-2.22-.253-4.555-1.113-4.555-4.951 0-1.093.39-1.988 1.029-2.688-.103-.253-.446-1.272.098-2.65 0 0 .84-.27 2.75 1.026A9.564 9.564 0 0112 6.844c.85.004 1.705.115 2.504.337 1.909-1.296 2.747-1.027 2.747-1.027.546 1.379.202 2.398.1 2.651.64.7 1.028 1.595 1.028 2.688 0 3.848-2.339 4.695-4.566 4.943.359.309.678.92.678 1.855 0 1.338-.012 2.419-.012 2.747 0 .268.18.58.688.482A10.019 10.019 0 0022 12.017C22 6.484 17.522 2 12 2z"/>
          </svg>
        </div>
        <div>
          <h1 class="text-sm sm:text-base font-bold text-white flex items-center gap-2">
            پیش‌نمایش زنده پروفایل گیت‌هاب
            <span class="text-xs font-normal px-2 py-0.5 rounded-full bg-cyan-500/15 text-cyan-300 border border-cyan-500/30">SSLRI</span>
          </h1>
          <p class="text-xs text-[#8b949e] hidden sm:block">تغییرات را بررسی کنید و کد آماده README.md را کپی نمایید</p>
        </div>
      </div>

      <!-- Controls Group -->
      <div class="flex flex-wrap items-center gap-2">
        
        <!-- Viewport Switcher (Desktop / Mobile) -->
        <div class="bg-[#0d1117] p-1 rounded-lg border border-[#30363d] flex items-center text-xs">
          <button id="btnDesktop" onclick="setViewport('desktop')" class="px-2.5 py-1.5 rounded-md font-medium transition flex items-center gap-1.5 bg-[#21262d] text-white shadow-sm">
            <svg class="w-4 h-4 text-cyan-400" fill="none" stroke="currentColor" viewBox="0 0 24 24"><rect x="2" y="3" width="20" height="14" rx="2" stroke-width="2"/><path d="M8 21h8M12 17v4" stroke-width="2" stroke-linecap="round"/></svg>
            <span>دسکتاپ</span>
          </button>
          <button id="btnMobile" onclick="setViewport('mobile')" class="px-2.5 py-1.5 rounded-md font-medium transition flex items-center gap-1.5 text-[#8b949e] hover:text-white">
            <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24"><rect x="5" y="2" width="14" height="20" rx="2" stroke-width="2"/><path d="M12 18h.01" stroke-width="2" stroke-linecap="round"/></svg>
            <span>موبایل</span>
          </button>
        </div>

        <!-- Theme Selector -->
        <div class="flex items-center gap-1.5 bg-[#0d1117] px-2.5 py-1.5 rounded-lg border border-[#30363d] text-xs">
          <span class="text-[#8b949e] hidden md:inline">تم رنگی هدر:</span>
          <select id="themeSelect" onchange="changeTheme(this.value)" class="bg-transparent text-white font-medium focus:outline-none cursor-pointer">
            <option value="tokyonight" class="bg-[#161b22]">Tokyo Night (پیشنهادی)</option>
            <option value="radical" class="bg-[#161b22]">Radical</option>
            <option value="dracula" class="bg-[#161b22]">Dracula</option>
            <option value="cyberpunk" class="bg-[#161b22]">Cyberpunk</option>
          </select>
        </div>

        <!-- Toggle Customizer Drawer -->
        <button onclick="toggleCustomizer()" class="px-3 py-1.5 rounded-lg bg-[#21262d] hover:bg-[#30363d] border border-[#30363d] text-xs font-medium text-white transition flex items-center gap-1.5">
          <svg class="w-4 h-4 text-amber-400" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 6V4m0 2a2 2 0 100 4m0-4a2 2 0 110 4m-6 8a2 2 0 100-4m0 4a2 2 0 110-4m0 4v2m0-6V4m6 6v10m6-2a2 2 0 100-4m0 4a2 2 0 110-4m0 4v2m0-6V4"/></svg>
          <span>ویرایش مهارت‌ها</span>
        </button>

        <!-- Toggle Raw Markdown Modal/View -->
        <button id="btnToggleRaw" onclick="toggleRawView()" class="px-3 py-1.5 rounded-lg bg-[#21262d] hover:bg-[#30363d] border border-[#30363d] text-xs font-medium text-white transition flex items-center gap-1.5">
          <svg class="w-4 h-4 text-purple-400" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M10 20l4-16m4 4l4 4-4 4M6 16l-4-4 4-4"/></svg>
          <span id="rawBtnText">مشاهده کد خام</span>
        </button>

        <!-- Copy Markdown CTA -->
        <button onclick="copyMarkdown()" class="px-3.5 py-1.5 rounded-lg bg-emerald-600 hover:bg-emerald-500 text-white text-xs font-semibold transition flex items-center gap-1.5 shadow-md shadow-emerald-900/30">
          <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24"><rect x="9" y="9" width="13" height="13" rx="2" stroke-width="2"/><path d="M5 15H4a2 2 0 01-2-2V4a2 2 0 012-2h9a2 2 0 012 2v1" stroke-width="2"/></svg>
          <span>کپی کد README.md</span>
        </button>

      </div>
    </div>

    <!-- Collapsible Skills & Profile Customizer Panel -->
    <div id="customizerPanel" class="hidden max-w-7xl mx-auto mt-3 pt-3 border-t border-[#30363d] text-xs">
      <div class="flex flex-col md:flex-row items-start md:items-center justify-between gap-4 bg-[#0d1117] p-3 rounded-xl border border-[#30363d]">
        <div>
          <span class="font-bold text-cyan-400 block mb-1">🛠️ انتخاب آیکون‌های بخش Tech Stack (با کلیک، هم پیش‌نمایش و هم کد خروجی آپدیت می‌شود):</span>
          <div id="skillCheckboxes" class="flex flex-wrap gap-2 mt-2">
            <!-- Populated by JS -->
          </div>
        </div>
      </div>
    </div>
  </header>

  <!-- Toast Notification -->
  <div id="toast" class="fixed bottom-5 left-5 z-50 transform translate-y-20 opacity-0 pointer-events-none transition-all duration-300 bg-emerald-600 text-white px-4 py-3 rounded-xl shadow-2xl flex items-center gap-2.5 border border-emerald-400/30 text-sm font-medium">
    <svg class="w-5 h-5 text-white shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5" d="M5 13l4 4L19 7"/></svg>
    <span id="toastMsg">کد README.md با موفقیت در کلیپ‌بورد کپی شد!</span>
  </div>

  <!-- ================= RAW MARKDOWN CODE VIEW (HIDDEN BY DEFAULT) ================= -->
  <section id="rawViewSection" class="hidden max-w-5xl w-full mx-auto px-4 py-6">
    <div class="bg-[#161b22] border border-[#30363d] rounded-xl overflow-hidden shadow-2xl">
      <div class="flex items-center justify-between px-4 py-3 bg-[#21262d] border-b border-[#30363d]">
        <div class="flex items-center gap-2 text-sm font-semibold text-white">
          <svg class="w-4 h-4 text-cyan-400" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12h6m-6 4h6m2 5H7a2 2 0 01-2-2V5a2 2 0 012-2h5.586a1 1 0 01.707.293l5.414 5.414a1 1 0 01.293.707V19a2 2 0 01-2 2z"/></svg>
          <span>کد نهایی فایل <code class="text-cyan-300 font-fira">SSLRI/README.md</code></span>
        </div>
        <div class="flex items-center gap-2">
          <button onclick="copyMarkdown()" class="px-3 py-1 rounded-lg bg-emerald-600 hover:bg-emerald-500 text-white text-xs font-medium transition">
            کپی کد
          </button>
          <button onclick="toggleRawView()" class="px-3 py-1 rounded-lg bg-[#30363d] hover:bg-[#484f58] text-white text-xs font-medium transition">
            بازگشت به پیش‌نمایش
          </button>
        </div>
      </div>
      <pre id="rawMarkdownOutput" dir="ltr" class="p-4 text-xs sm:text-sm font-fira text-[#c9d1d9] overflow-x-auto leading-relaxed select-all bg-[#0d1117]"></pre>
    </div>
  </section>

  <!-- ================= MAIN GITHUB LIVE PREVIEW CONTAINER ================= -->
  <main class="flex-1 px-2 sm:px-6 py-6">
    <div id="previewFrame" class="desktop-frame gh-ltr">
      
      <!-- Simulated GitHub Top Navigation Bar -->
      <div class="bg-[#161b22] border-b border-[#30363d] px-4 pt-3 rounded-t-xl">
        <div class="flex items-center justify-between mb-3">
          <div class="flex items-center gap-3">
            <button class="p-1.5 rounded-md border border-[#30363d] text-[#8b949e] hover:text-white">
              <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"/></svg>
            </button>
            <svg class="w-7 h-7 text-white" fill="currentColor" viewBox="0 0 24 24">
              <path fill-rule="evenodd" clip-rule="evenodd" d="M12 2C6.477 2 2 6.484 2 12.017c0 4.425 2.865 8.18 6.839 9.504.5.092.682-.217.682-.483 0-.237-.008-.868-.013-1.703-2.782.605-3.369-1.343-3.369-1.343-.454-1.158-1.11-1.466-1.11-1.466-.908-.62.069-.608.069-.608 1.003.07 1.53 1.032 1.53 1.032.892 1.53 2.341 1.088 2.91.832.092-.647.35-1.088.636-1.338-2.22-.253-4.555-1.113-4.555-4.951 0-1.093.39-1.988 1.029-2.688-.103-.253-.446-1.272.098-2.65 0 0 .84-.27 2.75 1.026A9.564 9.564 0 0112 6.844c.85.004 1.705.115 2.504.337 1.909-1.296 2.747-1.027 2.747-1.027.546 1.379.202 2.398.1 2.651.64.7 1.028 1.595 1.028 2.688 0 3.848-2.339 4.695-4.566 4.943.359.309.678.92.678 1.855 0 1.338-.012 2.419-.012 2.747 0 .268.18.58.688.482A10.019 10.019 0 0022 12.017C22 6.484 17.522 2 12 2z"/>
            </svg>
            <span class="font-semibold text-sm text-white">SSLRI</span>
          </div>
          <div class="flex items-center gap-2">
            <div class="hidden sm:flex items-center gap-2 px-2.5 py-1 rounded-md border border-[#30363d] text-xs text-[#8b949e]">
              <svg class="w-3.5 h-3.5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"/></svg>
              <span>Type <kbd class="px-1 border border-[#30363d] rounded text-[10px]">/</kbd> to search</span>
            </div>
            <div class="w-7 h-7 rounded-full bg-gradient-to-tr from-emerald-500 to-cyan-500 p-0.5">
              <div class="w-full h-full rounded-full bg-[#0d1117] flex items-center justify-center text-[11px] font-bold text-cyan-400">SS</div>
            </div>
          </div>
        </div>

        <!-- GitHub Profile Tabs -->
        <div class="flex items-center gap-5 text-xs sm:text-sm overflow-x-auto no-scrollbar">
          <a href="#overview" onclick="return false" class="flex items-center gap-2 py-2.5 border-b-2 border-[#f78166] font-semibold text-white whitespace-nowrap">
            <svg class="w-4 h-4 text-[#8b949e]" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 6.253v13m0-13C10.832 5.477 9.246 5 7.5 5S4.168 5.477 3 6.253v13C4.168 18.477 5.754 18 7.5 18s3.332.477 4.5 1.253m0-13C13.168 5.477 14.754 5 16.5 5c1.747 0 3.332.477 4.5 1.253v13C19.832 18.477 18.247 18 16.5 18c-1.746 0-3.332.477-4.5 1.253"/></svg>
            Overview
          </a>
          <a href="#repos" onclick="return false" class="flex items-center gap-1.5 py-2.5 text-[#8b949e] hover:text-white whitespace-nowrap">
            <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 7v10a2 2 0 002 2h14a2 2 0 002-2V9a2 2 0 00-2-2h-6l-2-2H5a2 2 0 00-2 2z"/></svg>
            Repositories
            <span class="px-1.5 py-0.2 rounded-full bg-[#30363d] text-[#c9d1d9] text-xs">9</span>
          </a>
          <a href="#projects" onclick="return false" class="flex items-center gap-1.5 py-2.5 text-[#8b949e] hover:text-white whitespace-nowrap">
            <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 17V7m0 10a2 2 0 01-2 2H5a2 2 0 01-2-2V7a2 2 0 012-2h2a2 2 0 012 2m0 10a2 2 0 002 2h2a2 2 0 002-2M9 7a2 2 0 012-2h2a2 2 0 012 2m0 10V7"/></svg>
            Projects
          </a>
          <a href="#stars" onclick="return false" class="flex items-center gap-1.5 py-2.5 text-[#8b949e] hover:text-white whitespace-nowrap">
            <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M11.049 2.927c.3-.921 1.603-.921 1.902 0l1.519 4.674a1 1 0 00.95.69h4.915c.969 0 1.371 1.24.588 1.81l-3.976 2.888a1 1 0 00-.363 1.118l1.518 4.674c.3.922-.755 1.688-1.538 1.118l-3.976-2.888a1 1 0 00-1.176 0l-3.976 2.888c-.783.57-1.838-.197-1.538-1.118l1.518-4.674a1 1 0 00-.363-1.118l-3.976-2.888c-.784-.57-.38-1.81.588-1.81h4.914a1 1 0 00.951-.69l1.519-4.674z"/></svg>
            Stars
          </a>
        </div>
      </div>

      <!-- GitHub Profile Main Grid -->
      <div id="profileGrid" class="bg-[#0d1117] border-x border-b border-[#30363d] rounded-b-xl p-4 sm:p-6 grid grid-cols-1 lg:grid-cols-12 gap-6">
        
        <!-- LEFT SIDEBAR: User Profile Info -->
        <aside id="profileSidebar" class="lg:col-span-3 flex flex-col gap-4">
          
          <!-- Avatar + Name Group -->
          <div id="avatarGroup" class="flex sm:flex-row lg:flex-col items-center sm:items-start gap-4">
            <div class="relative group shrink-0">
              <!-- Stylish Avatar matching user photo vibe -->
              <div class="w-20 h-20 sm:w-28 sm:h-28 lg:w-60 lg:h-60 rounded-full border-2 border-[#30363d] overflow-hidden bg-gradient-to-b from-emerald-900/40 to-[#161b22] flex items-center justify-center shadow-xl">
                <svg viewBox="0 0 200 200" class="w-full h-full">
                  <defs>
                    <linearGradient id="bgGrad" x1="0%" y1="0%" x2="100%" y2="100%">
                      <stop offset="0%" stop-color="#1e3a2f"/>
                      <stop offset="50%" stop-color="#0f2926"/>
                      <stop offset="100%" stop-color="#0d1117"/>
                    </linearGradient>
                    <linearGradient id="shirtGrad" x1="0%" y1="0%" x2="100%" y2="0%">
                      <stop offset="0%" stop-color="#f48fb1"/>
                      <stop offset="100%" stop-color="#ec407a"/>
                    </linearGradient>
                  </defs>
                  <!-- Nature / Foliage blurred background -->
                  <rect width="200" height="200" fill="url(#bgGrad)"/>
                  <circle cx="35" cy="45" r="28" fill="#2e7d32" opacity="0.35"/>
                  <circle cx="165" cy="50" r="35" fill="#4caf50" opacity="0.25"/>
                  <circle cx="150" cy="20" r="20" fill="#81c784" opacity="0.3"/>
                  <!-- Shoulders / Pink Shirt -->
                  <path d="M35 200 C35 148, 165 148, 165 200 Z" fill="url(#shirtGrad)"/>
                  <!-- Collar -->
                  <path d="M72 152 L100 178 L128 152 L118 145 L100 165 L82 145 Z" fill="#f8bbd0"/>
                  <!-- Neck -->
                  <rect x="85" y="125" width="30" height="32" rx="10" fill="#d7a184"/>
                  <!-- Head -->
                  <rect x="68" y="56" width="64" height="78" rx="30" fill="#e0ac8b"/>
                  <!-- Beard & Mustache -->
                  <path d="M68 98 C68 128, 85 138, 100 138 C115 138, 132 128, 132 98 C128 112, 118 122, 100 122 C82 122, 72 112, 68 98 Z" fill="#1f1b18"/>
                  <path d="M84 112 Q100 106 116 112 Q100 117 84 112 Z" fill="#1f1b18"/>
                  <!-- Smile -->
                  <path d="M90 116 Q100 123 110 116" stroke="#fff" stroke-width="2.5" fill="none" stroke-linecap="round"/>
                  <!-- Eyes & Eyebrows -->
                  <circle cx="85" cy="88" r="4" fill="#1a1a1a"/>
                  <circle cx="115" cy="88" r="4" fill="#1a1a1a"/>
                  <path d="M76 80 Q85 76 93 80" stroke="#1f1b18" stroke-width="3.2" fill="none" stroke-linecap="round"/>
                  <path d="M107 80 Q115 76 124 80" stroke="#1f1b18" stroke-width="3.2" fill="none" stroke-linecap="round"/>
                  <!-- Hair -->
                  <path d="M65 82 C62 52, 85 40, 102 42 C125 42, 138 56, 135 82 C130 64, 115 58, 100 58 C82 58, 70 66, 65 82 Z" fill="#1a1615"/>
                </svg>
              </div>
            </div>

            <div class="pt-1">
              <h2 class="text-xl sm:text-2xl font-bold text-white leading-tight">Saeed Salari</h2>
              <p class="text-base sm:text-lg text-[#8b949e] font-light">SSLRI</p>
            </div>
          </div>

          <!-- Status Box (Fixed Spelling: respond) -->
          <div class="flex items-center justify-between gap-2 px-3 py-2 rounded-lg border border-[#30363d] bg-[#161b22]/60 text-xs text-[#c9d1d9]">
            <div class="flex items-center gap-2">
              <span class="text-base">😊</span>
              <span>I may be slow to <strong class="text-emerald-400 underline decoration-dotted" title="اصلاح شده از responce به respond">respond</strong></span>
            </div>
            <span class="text-[10px] px-1.5 py-0.5 rounded bg-emerald-500/10 text-emerald-400 border border-emerald-500/20">اصلاح املایی</span>
          </div>

          <!-- Bio -->
          <p class="text-sm text-[#c9d1d9] leading-relaxed">
            Co-Founder &amp; CEO of Iran YouSec | Curious mind exploring the depths of cybersecurity and technology.
          </p>

          <!-- Edit Profile Button -->
          <button class="w-full py-1.5 px-3 rounded-md bg-[#21262d] hover:bg-[#30363d] border border-[#30363d] text-xs font-semibold text-[#c9d1d9] transition">
            Edit profile
          </button>

          <!-- Links & Socials -->
          <div class="flex flex-col gap-2 text-xs sm:text-sm text-[#c9d1d9] pt-1">
            <div class="flex items-center gap-2">
              <svg class="w-4 h-4 text-[#8b949e] shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13.828 10.172a4 4 0 00-5.656 0l-4 4a4 4 0 105.656 5.656l1.102-1.101m-.758-4.899a4 4 0 005.656 0l4-4a4 4 0 00-5.656-5.656l-1.1 1.1"/></svg>
              <a href="https://www.sslri.ir" target="_blank" class="hover:text-[#58a6ff] hover:underline truncate">https://www.sslri.ir</a>
            </div>
            <div class="flex items-center gap-2">
              <svg class="w-4 h-4 text-[#8b949e] shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13.828 10.172a4 4 0 00-5.656 0l-4 4a4 4 0 105.656 5.656l1.102-1.101m-.758-4.899a4 4 0 005.656 0l4-4a4 4 0 00-5.656-5.656l-1.1 1.1"/></svg>
              <a href="https://t.me/sslri" target="_blank" class="hover:text-[#58a6ff] hover:underline truncate">https://T.me/sslri</a>
            </div>
            <div class="flex items-center gap-2">
              <svg class="w-4 h-4 text-[#8b949e] shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24"><rect x="2" y="2" width="20" height="20" rx="5" stroke-width="2"/><circle cx="12" cy="12" r="4" stroke-width="2"/><circle cx="17.5" cy="6.5" r="1" fill="currentColor"/></svg>
              <a href="https://instagram.com/sslri" target="_blank" class="hover:text-[#58a6ff] hover:underline truncate">https://Instagram.com/sslri</a>
            </div>
          </div>

          <!-- Followers / Following -->
          <div class="flex items-center gap-1.5 text-xs text-[#8b949e] pt-1">
            <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 20h5v-2a3 3 0 00-5.356-1.857M17 20H7m10 0v-2c0-.656-.126-1.283-.356-1.857M7 20H2v-2a3 3 0 015.356-1.857M7 20v-2c0-.656.126-1.283.356-1.857m0 0a5.002 5.002 0 019.288 0M15 7a3 3 0 11-6 0 3 3 0 016 0z"/></svg>
            <span class="font-bold text-white">58</span> followers
            <span>·</span>
            <span class="font-bold text-white">0</span> following
          </div>

          <hr class="border-[#30363d] my-1" />

          <!-- Achievements -->
          <div>
            <h3 class="text-sm font-semibold text-white mb-2.5">Achievements</h3>
            <div class="flex items-center gap-2.5">
              <!-- Pull Shark SVG Badge -->
              <div class="w-14 h-14 rounded-full bg-gradient-to-b from-blue-500 to-indigo-900 p-0.5 shadow-md" title="Pull Shark">
                <div class="w-full h-full rounded-full bg-[#0c2d6b] flex items-center justify-center relative overflow-hidden">
                  <svg viewBox="0 0 64 64" class="w-11 h-11">
                    <circle cx="32" cy="32" r="28" fill="#1d4ed8" opacity="0.4"/>
                    <path d="M18 38 C20 22, 32 14, 44 24 C48 28, 48 36, 44 42 C36 38, 26 38, 18 38 Z" fill="#60a5fa"/>
                    <path d="M24 34 Q32 40 40 34" stroke="#fff" stroke-width="2.5" fill="none" stroke-linecap="round"/>
                    <circle cx="26" cy="26" r="2.5" fill="#0f172a"/>
                    <circle cx="38" cy="26" r="2.5" fill="#0f172a"/>
                    <rect x="26" y="40" width="12" height="10" rx="2" fill="#e2e8f0"/>
                  </svg>
                </div>
              </div>
              <!-- Starstruck SVG Badge -->
              <div class="w-14 h-14 rounded-full bg-gradient-to-tr from-amber-400 via-pink-500 to-purple-600 p-0.5 shadow-md" title="Starstruck">
                <div class="w-full h-full rounded-full bg-[#1e1b4b] flex items-center justify-center">
                  <svg viewBox="0 0 64 64" class="w-11 h-11">
                    <circle cx="32" cy="34" r="18" fill="#fbbf24"/>
                    <!-- Star Eyes -->
                    <polygon points="24,26 26,30 30,30 27,33 28,37 24,34 20,37 21,33 18,30 22,30" fill="#fef08a" stroke="#b45309" stroke-width="1"/>
                    <polygon points="40,26 42,30 46,30 43,33 44,37 40,34 36,37 37,33 34,30 38,30" fill="#fef08a" stroke="#b45309" stroke-width="1"/>
                    <path d="M24 41 Q32 48 40 41 Z" fill="#78350f"/>
                  </svg>
                </div>
              </div>
            </div>
          </div>

        </aside>

        <!-- RIGHT MAIN CONTENT: SSLRI / README.md Box -->
        <section id="readmeColumn" class="lg:col-span-9">
          <div class="border border-[#30363d] rounded-xl bg-[#0d1117] p-4 sm:p-7 shadow-inner">
            
            <!-- Top path header: SSLRI / README.md -->
            <div class="flex items-center justify-between pb-4 mb-5 border-b border-[#21262d] text-xs text-[#8b949e]">
              <span class="font-mono">SSLRI / <strong class="text-white">README.md</strong></span>
              <button onclick="copyMarkdown()" class="text-[#8b949e] hover:text-white flex items-center gap-1 transition" title="Copy Markdown">
                <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15.232 5.232l3.536 3.536m-2.036-5.036a2.5 2.5 0 113.536 3.536L6.5 21.036H3v-3.572L16.732 3.732z"/></svg>
              </button>
            </div>

            <!-- ==================== ACTUAL RENDERED README CONTENT ==================== -->
            <div class="space-y-7">
              
              <!-- 1. Upgraded Hero Header Block (Above About Me) -->
              <div class="text-center space-y-5">
                
                <!-- High-Graphics Animated Cyber Banner (Capsule Render Simulation) -->
                <div class="relative rounded-2xl overflow-hidden border border-[#30363d] shadow-2xl bg-[#0d1117] group">
                  <svg viewBox="0 0 850 220" class="w-full h-auto block">
                    <defs>
                      <linearGradient id="heroGrad" x1="0%" y1="0%" x2="100%" y2="100%">
                        <stop offset="0%" stop-color="#090d16"/>
                        <stop offset="45%" stop-color="#111c35"/>
                        <stop offset="80%" stop-color="#0f2942"/>
                        <stop offset="100%" stop-color="#083344"/>
                      </linearGradient>
                      <linearGradient id="waveGrad1" x1="0%" y1="0%" x2="100%" y2="0%">
                        <stop offset="0%" stop-color="#00f7ff" stop-opacity="0.18"/>
                        <stop offset="50%" stop-color="#6366f1" stop-opacity="0.25"/>
                        <stop offset="100%" stop-color="#00f7ff" stop-opacity="0.15"/>
                      </linearGradient>
                      <linearGradient id="waveGrad2" x1="0%" y1="0%" x2="100%" y2="0%">
                        <stop offset="0%" stop-color="#3b82f6" stop-opacity="0.12"/>
                        <stop offset="50%" stop-color="#00f7ff" stop-opacity="0.28"/>
                        <stop offset="100%" stop-color="#8b5cf6" stop-opacity="0.12"/>
                      </linearGradient>
                      <linearGradient id="accentGlow" x1="0%" y1="0%" x2="100%" y2="0%">
                        <stop offset="0%" stop-color="transparent"/>
                        <stop offset="50%" stop-color="#00f7ff"/>
                        <stop offset="100%" stop-color="transparent"/>
                      </linearGradient>
                      <pattern id="cyberGrid" width="32" height="32" patternUnits="userSpaceOnUse">
                        <path d="M 32 0 L 0 0 0 32" fill="none" stroke="#00f7ff" stroke-width="0.6" stroke-opacity="0.07"/>
                      </pattern>
                    </defs>

                    <!-- Base Background + Cyber Grid -->
                    <rect width="850" height="220" fill="url(#heroGrad)"/>
                    <rect width="850" height="220" fill="url(#cyberGrid)"/>

                    <!-- Glowing Orbs -->
                    <circle cx="140" cy="50" r="90" fill="#00f7ff" opacity="0.08" class="glow-pulse"/>
                    <circle cx="720" cy="60" r="110" fill="#6366f1" opacity="0.1" class="glow-pulse"/>

                    <!-- Decorative Cyber Nodes (Left & Right) -->
                    <g stroke="#00f7ff" stroke-opacity="0.3" stroke-width="1.2" fill="none">
                      <polyline points="25,40 65,40 85,60 130,60"/>
                      <circle cx="25" cy="40" r="3" fill="#00f7ff"/>
                      <circle cx="130" cy="60" r="2.5" fill="#00f7ff"/>
                      <polyline points="825,45 780,45 760,65 715,65"/>
                      <circle cx="825" cy="45" r="3" fill="#00f7ff"/>
                      <circle cx="715" cy="65" r="2.5" fill="#00f7ff"/>
                    </g>

                    <!-- Layered Smooth Cyber Waves -->
                    <path d="M0,155 C220,210 380,105 600,160 C720,190 800,145 850,155 L850,220 L0,220 Z" fill="url(#waveGrad1)"/>
                    <path d="M0,175 C180,130 410,215 640,155 C740,130 810,170 850,180 L850,220 L0,220 Z" fill="url(#waveGrad2)"/>
                    <path d="M0,195 C280,170 520,215 850,185 L850,220 L0,220 Z" fill="#0d1117" opacity="0.85"/>

                    <!-- Main Title & Subtitle -->
                    <text x="425" y="92" text-anchor="middle" fill="#ffffff" font-family="Inter, sans-serif" font-weight="800" font-size="36" letter-spacing="0.5">
                      Saeed Salari <tspan id="bannerAccentText" fill="#00f7ff">(SSLRI)</tspan>
                    </text>
                    <text x="425" y="128" text-anchor="middle" fill="#c9d1d9" font-family="Fira Code, monospace" font-weight="500" font-size="14.5" letter-spacing="0.4">
                      🛡️ Co-Founder &amp; CEO at Iran YouSec  •  ⚡ Cybersecurity &amp; Automation
                    </text>

                    <!-- Bottom Glowing Line -->
                    <rect x="225" y="146" width="400" height="1.5" fill="url(#accentGlow)" opacity="0.7"/>
                  </svg>
                </div>

                <!-- Terminal-Styled Animated Typing Bar -->
                <div class="inline-flex items-center justify-center gap-2.5 px-5 py-2.5 rounded-xl bg-[#161b22]/90 border border-[#30363d] shadow-inner min-h-[46px] max-w-full">
                  <span class="font-fira text-xs sm:text-sm font-bold text-emerald-400 select-none">root@sslri:~#</span>
                  <div class="flex items-center overflow-hidden">
                    <span id="typingText" class="font-fira font-semibold text-sm sm:text-lg md:text-xl tracking-tight truncate" style="color: #00F7FF;">
                      Hi there 👋, I'm Saeed Salari (SSLRI)
                    </span>
                    <span id="typingCursor" class="typing-cursor" style="background-color: #00F7FF;"></span>
                  </div>
                </div>

                <!-- Upgraded Glass/Dark Social & Status Badges Dock -->
                <div class="flex flex-wrap items-center justify-center gap-2.5 pt-1">
                  <!-- Website Badge -->
                  <a href="https://www.sslri.ir" target="_blank" class="group inline-flex items-center rounded-lg overflow-hidden border border-[#30363d] hover:border-[#0A66C2] shadow-md transition-all duration-200 transform hover:-translate-y-0.5 text-[11px] font-bold tracking-wider uppercase">
                    <span class="bg-[#161b22] text-[#c9d1d9] px-2.5 py-2 flex items-center gap-1.5">
                      <svg class="w-3.5 h-3.5 text-[#0A66C2]" fill="currentColor" viewBox="0 0 24 24"><path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm-1 17.93c-3.95-.49-7-3.85-7-7.93 0-.62.08-1.21.21-1.79L9 15v1c0 1.1.9 2 2 2v1.93zm6.9-2.54c-.26-.81-1-1.39-1.9-1.39h-1v-3c0-.55-.45-1-1-1H8v-2h2c.55 0 1-.45 1-1V7h2c1.1 0 2-.9 2-2v-.41c2.93 1.19 5 4.06 5 7.41 0 2.08-.8 3.97-2.1 5.39z"/></svg>
                      WEBSITE
                    </span>
                    <span class="bg-gradient-to-r from-[#0A66C2] to-[#0284c7] text-white px-3 py-2">SSLRI.IR</span>
                  </a>

                  <!-- Telegram Badge -->
                  <a href="https://t.me/sslri" target="_blank" class="group inline-flex items-center rounded-lg overflow-hidden border border-[#30363d] hover:border-[#26A5E4] shadow-md transition-all duration-200 transform hover:-translate-y-0.5 text-[11px] font-bold tracking-wider uppercase">
                    <span class="bg-[#161b22] text-[#c9d1d9] px-2.5 py-2 flex items-center gap-1.5">
                      <svg class="w-3.5 h-3.5 text-[#26A5E4]" fill="currentColor" viewBox="0 0 24 24"><path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm4.64 6.8c-.15 1.58-.8 5.42-1.13 7.19-.14.75-.42 1-.68 1.03-.58.05-1.02-.38-1.58-.75-.88-.58-1.38-.94-2.23-1.5-.99-.65-.35-1.01.22-1.59.15-.15 2.71-2.48 2.76-2.69.01-.03.01-.14-.07-.2-.08-.06-.19-.04-.27-.02-.12.02-1.96 1.25-5.54 3.69-.52.36-1 .53-1.42.52-.47-.01-1.37-.26-2.03-.48-.82-.27-1.47-.42-1.42-.88.03-.24.35-.49.96-.75 3.78-1.65 6.31-2.74 7.58-3.27 3.61-1.51 4.35-1.77 4.84-1.78.11 0 .35.03.5.16.13.1.17.24.18.34.02.07.02.21.01.33z"/></svg>
                      TELEGRAM
                    </span>
                    <span class="bg-gradient-to-r from-[#26A5E4] to-[#0ea5e9] text-white px-3 py-2">@SSLRI</span>
                  </a>

                  <!-- Instagram Badge -->
                  <a href="https://instagram.com/sslri" target="_blank" class="group inline-flex items-center rounded-lg overflow-hidden border border-[#30363d] hover:border-[#E4405F] shadow-md transition-all duration-200 transform hover:-translate-y-0.5 text-[11px] font-bold tracking-wider uppercase">
                    <span class="bg-[#161b22] text-[#c9d1d9] px-2.5 py-2 flex items-center gap-1.5">
                      <svg class="w-3.5 h-3.5 text-[#E4405F]" fill="currentColor" viewBox="0 0 24 24"><rect x="2" y="2" width="20" height="20" rx="5"/></svg>
                      INSTAGRAM
                    </span>
                    <span class="bg-gradient-to-r from-[#E4405F] to-[#db2777] text-white px-3 py-2">@SSLRI</span>
                  </a>

                  <!-- Profile Views Badge -->
                  <div class="inline-flex items-center rounded-lg overflow-hidden border border-[#30363d] shadow-md text-[11px] font-bold tracking-wider uppercase">
                    <span class="bg-[#161b22] text-[#c9d1d9] px-2.5 py-2 flex items-center gap-1.5">
                      <svg class="w-3.5 h-3.5 text-cyan-400" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 12a3 3 0 11-6 0 3 3 0 016 0z"/><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M2.458 12C3.732 7.943 7.523 5 12 5c4.478 0 8.268 2.943 9.542 7-1.274 4.057-5.064 7-9.542 7-4.477 0-8.268-2.943-9.542-7z"/></svg>
                      VIEWS
                    </span>
                    <span id="viewsBadgeColor" class="bg-[#00f7ff] text-[#0d1117] font-extrabold px-3 py-2 font-mono">1,428</span>
                  </div>
                </div>

              </div>

              <hr class="border-[#21262d]" />

              <!-- 2. About Me Section with Animated dev.gif replacement -->
              <div>
                <h3 class="text-lg sm:text-xl font-semibold text-white mb-4 pb-2 border-b border-[#21262d]">
                  👨‍💻 About Me
                </h3>
                
                <div class="flex flex-col-reverse md:flex-row items-center justify-between gap-6">
                  <!-- Bullet Points -->
                  <ul class="space-y-2.5 text-sm sm:text-[15px] text-[#c9d1d9] list-disc list-inside flex-1 leading-relaxed">
                    <li>🛡️ <strong class="text-white">Co-Founder &amp; CEO</strong> at <strong class="text-white">Iran YouSec</strong></li>
                    <li>🔍 Curious mind exploring the depths of <strong class="text-white">Cybersecurity</strong>, <strong class="text-white">Network Security</strong>, and <strong class="text-white">Technology</strong></li>
                    <li>⚙️ Experienced in <strong class="text-white">Linux Server Administration</strong>, <strong class="text-white">Bash Scripting</strong>, and <strong class="text-white">Task Automation</strong></li>
                    <li>🤖 Building smart <strong class="text-white">Telegram Bots</strong>, CLI tools, and security utilities</li>
                    <li>🌐 Portfolio &amp; Updates: <a href="https://www.sslri.ir" target="_blank" class="text-[#58a6ff] font-semibold hover:underline">sslri.ir</a></li>
                  </ul>

                  <!-- Animated SVG representing ./dev.gif -->
                  <div class="w-60 sm:w-64 shrink-0 relative">
                    <div class="rounded-xl bg-[#161b22] border border-[#30363d] p-3 shadow-lg relative overflow-hidden">
                      <span class="absolute top-2 right-2 text-[10px] font-mono px-1.5 py-0.5 rounded bg-cyan-500/10 text-cyan-400 border border-cyan-500/20">./dev.gif</span>
                      <svg viewBox="0 0 260 190" class="w-full h-auto dev-float">
                        <!-- Ambient Cyber Glow -->
                        <circle cx="130" cy="95" r="70" fill="#00f7ff" opacity="0.07" class="glow-pulse"/>
                        
                        <!-- Floating Terminal Window Left -->
                        <g class="code-anim">
                          <rect x="14" y="20" width="95" height="58" rx="6" fill="#0d1117" stroke="#30363d" stroke-width="1.5"/>
                          <circle cx="24" cy="29" r="2.5" fill="#ff5f56"/>
                          <circle cx="32" cy="29" r="2.5" fill="#ffbd2e"/>
                          <circle cx="40" cy="29" r="2.5" fill="#27c93f"/>
                          <rect x="22" y="39" width="45" height="4" rx="2" fill="#00f7ff" opacity="0.8"/>
                          <rect x="22" y="48" width="68" height="4" rx="2" fill="#7aa2f7" opacity="0.6"/>
                          <rect x="22" y="57" width="35" height="4" rx="2" fill="#9ece6a" opacity="0.8"/>
                          <rect x="22" y="66" width="55" height="4" rx="2" fill="#bb9af7" opacity="0.6"/>
                        </g>

                        <!-- Floating Cyber Shield Icon Right -->
                        <g transform="translate(185, 22)" class="glow-pulse">
                          <path d="M25 4 L45 12 V26 C45 40 35 50 25 55 C15 50 5 40 5 26 V12 L25 4 Z" fill="#00f7ff" fill-opacity="0.12" stroke="#00f7ff" stroke-width="1.8"/>
                          <path d="M18 29 L23 34 L33 23" stroke="#00f7ff" stroke-width="2.5" fill="none" stroke-linecap="round" stroke-linejoin="round"/>
                        </g>

                        <!-- Desk -->
                        <rect x="20" y="160" width="220" height="6" rx="3" fill="#30363d"/>

                        <!-- Developer Character -->
                        <circle cx="130" cy="88" r="18" fill="#e0ac8b"/>
                        <!-- Hoodie / Body -->
              <!-- 3. Tech Stack & Tools Section (High-Graphics 3D Squircle Icons) -->
              <div>
                <div class="flex items-center justify-between mb-4 pb-2 border-b border-[#21262d]">
                  <div class="flex items-center gap-2">
                    <h3 class="text-lg sm:text-xl font-semibold text-white">
                      🛠️ Tech Stack &amp; Cyber Arsenal
                    </h3>
                    <span class="text-[11px] px-2 py-0.5 rounded-full bg-cyan-500/10 text-cyan-400 border border-cyan-500/20 font-mono">High-Res Icons</span>
                  </div>
                  <button onclick="toggleCustomizer()" class="text-xs text-cyan-400 hover:underline font-sans flex items-center gap-1">
                    <span>+ ویرایش ابزارها</span>
                  </button>
                </div>

                <!-- Dynamic High-Graphics Skill Icons Showcase -->
                <div class="rounded-2xl bg-[#161b22]/60 border border-[#30363d] p-5 shadow-inner">
                  <div id="techStackGrid" class="flex flex-wrap items-center justify-center gap-3.5 sm:gap-4">
                    <!-- Populated via JS with High-Resolution Vector SVGs & 3D Gloss -->
                  </div>
                </div>
              </div>

              <hr class="border-[#21262d]" />

              <!-- 3. Tech Stack & Tools Section -->
              <div>
                <div class="flex items-center justify-between mb-4 pb-2 border-b border-[#21262d]">
                  <h3 class="text-lg sm:text-xl font-semibold text-white">
                    🛠️ Tech Stack &amp; Tools
                  </h3>
                  <button onclick="toggleCustomizer()" class="text-xs text-cyan-400 hover:underline font-sans">
                    + تغییر آیکون‌ها
                  </button>
                </div>

                <!-- Dynamic Skill Icons Grid -->
                <div id="techStackGrid" class="flex flex-wrap items-center justify-center gap-3 py-2">
                  <!-- Populated via JS -->
                </div>
              </div>

              <hr class="border-[#21262d]" />

              <!-- 4. Footer Quote -->
              <div class="text-center pt-1 pb-2">
                <span class="text-xs sm:text-sm text-[#8b949e] italic">
                  ⚡ "Security is not a product, but a process."
                </span>
              </div>

            </div>
            <!-- ==================== END RENDERED README CONTENT ==================== -->

          </div>
        </section>

      </div>
    </div>
  </main>

  <!-- ================= JAVASCRIPT LOGIC ================= -->
  <script>
    // 1. Typing Animation Phrases
    const phrases = [
      "Hi there 👋, I'm Saeed Salari (SSLRI)",
      "Co-Founder & CEO of Iran YouSec",
      "Cybersecurity Enthusiast & Tech Explorer",
      "Automation & Linux Administration"
    ];
    let phraseIdx = 0;
    let charIdx = 0;
    let isDeleting = false;
    const typingEl = document.getElementById('typingText');

    function typeLoop() {
      const currentPhrase = phrases[phraseIdx];
      if (isDeleting) {
        charIdx--;
      } else {
        charIdx++;
      }

      typingEl.textContent = currentPhrase.substring(0, charIdx);

      let speed = isDeleting ? 35 : 70;

      if (!isDeleting && charIdx === currentPhrase.length) {
        speed = 1800; // Pause at full sentence
        isDeleting = true;
      } else if (isDeleting && charIdx === 0) {
        isDeleting = false;
        phraseIdx = (phraseIdx + 1) % phrases.length;
        speed = 400;
      }

      setTimeout(typeLoop, speed);
    }

    // 2. High-Resolution Vector SVG Artwork for Every Skill (3D SkillIcons Style)
    const allSkills = [
      {
        id: 'linux',
        name: 'Linux',
        glow: '#FCC624',
        active: true,
        svg: `<svg viewBox="0 0 64 64" class="w-10 h-10"><rect width="64" height="64" rx="14" fill="#1e2229"/><path d="M32 10c-7 0-11 5.5-11 13 0 4.5-4 10-4 17 0 6 4.5 11 15 11s15-5 15-11c0-7-4-12.5-4-17 0-7.5-4-13-11-13z" fill="#111317"/><ellipse cx="32" cy="36" rx="9.5" ry="12.5" fill="#f8fafc"/><circle cx="28.5" cy="21" r="2.6" fill="#fff"/><circle cx="35.5" cy="21" r="2.6" fill="#fff"/><circle cx="29" cy="21.2" r="1.2" fill="#000"/><circle cx="35" cy="21.2" r="1.2" fill="#000"/><path d="M27 25.5c2-1.5 8-1.5 10 0l-5 4.2-5-4.2z" fill="#f59e0b"/><ellipse cx="23" cy="49" rx="5.5" ry="3.2" transform="rotate(-12 23 49)" fill="#f59e0b"/><ellipse cx="41" cy="49" rx="5.5" ry="3.2" transform="rotate(12 41 49)" fill="#f59e0b"/></svg>`
      },
      {
        id: 'bash',
        name: 'Bash',
        glow: '#4EAA25',
        active: true,
        svg: `<svg viewBox="0 0 64 64" class="w-10 h-10"><rect width="64" height="64" rx="14" fill="#1c242b"/><path d="M12 16a4 4 0 014-4h32a4 4 0 014 4v32a4 4 0 01-4 4H16a4 4 0 01-4-4V16z" fill="#232d36" stroke="#4EAA25" stroke-width="1.5" stroke-opacity="0.5"/><path d="M20 24l9 7-9 7" stroke="#4EAA25" stroke-width="3.8" stroke-linecap="round" stroke-linejoin="round" fill="none"/><line x1="32" y1="40" x2="44" y2="40" stroke="#fff" stroke-width="3.8" stroke-linecap="round"/></svg>`
      },
      {
        id: 'py',
        name: 'Python',
        glow: '#38bdf8',
        active: true,
        svg: `<svg viewBox="0 0 64 64" class="w-10 h-10"><rect width="64" height="64" rx="14" fill="#182232"/><path d="M31.5 11c-9 0-8.5 4-8.5 4v4.5h9v1.8H19.5S12 20.5 12 29.8c0 9.3 6.5 9 6.5 9h3.8v-4.4s-.2-5.4 5.3-5.4h9.2s5.1.1 5.1-4.9v-8.3S42.7 11 31.5 11zm-5 3.2a1.7 1.7 0 110 3.4 1.7 1.7 0 010-3.4z" fill="#387eb8"/><path d="M32.5 53c9 0 8.5-4 8.5-4v-4.5h-9v-1.8h12.5S52 43.5 52 34.2c0-9.3-6.5-9-6.5-9h-3.8v4.4s.2 5.4-5.3 5.4h-9.2s-5.1-.1-5.1 4.9v8.3S21.3 53 32.5 53zm5-3.2a1.7 1.7 0 110-3.4 1.7 1.7 0 010 3.4z" fill="#ffe052"/></svg>`
      },
      {
        id: 'js',
        name: 'JavaScript',
        glow: '#F7DF1E',
        active: true,
        svg: `<svg viewBox="0 0 64 64" class="w-10 h-10"><rect width="64" height="64" rx="14" fill="#F7DF1E"/><path d="M29 46.5v-18h4.8v18.2c0 3.5-2.1 5.3-5.6 5.3-2.8 0-4.6-1.4-5.5-3.4l4-2.4c.4.8.9 1.4 1.6 1.4.8 0 1.2-.5 1.2-1.6v.5zm15.8 5.5c-3.6 0-6-1.7-7.2-4.1l4-2.3c.9 1.5 2.1 2.5 4 2.5 1.7 0 2.7-.8 2.7-2 0-1.4-1.1-1.9-3-2.7l-1-.4c-3-1.3-5-2.9-5-6.3 0-3.1 2.4-5.5 6.1-5.5 2.7 0 4.6.9 6 3.3l-3.8 2.4c-.7-1.3-1.5-1.8-2.6-1.8-1.2 0-2 .8-2 1.8 0 1.2.8 1.7 2.6 2.5l1 .4c3.5 1.5 5.5 3.1 5.5 6.6 0 3.8-3 5.6-7.3 5.6z" fill="#111"/></svg>`
      },
      {
        id: 'html',
        name: 'HTML5',
        glow: '#E34F26',
        active: true,
        svg: `<svg viewBox="0 0 64 64" class="w-10 h-10"><rect width="64" height="64" rx="14" fill="#231715"/><polygon points="16,12 48,12 45,48 32,52 19,48" fill="#E34F26"/><polygon points="32,15 44.8,15 42.3,45.5 32,48.5" fill="#EF652A"/><polygon points="32,23 22,23 23,34 32,34 32,29.5 27,29.5 26.7,27 32,27" fill="#ebebeb"/><polygon points="32,39.5 27.5,38.2 27.2,35.5 23,35.5 23.6,41.8 32,44.2" fill="#ebebeb"/><polygon points="32,23 42,23 41.6,27 32,27" fill="#fff"/><polygon points="32,29.5 41.2,29.5 40.2,41.8 32,44.2 32,39.5 36.5,38.2 37,34 32,34" fill="#fff"/></svg>`
      },
      {
        id: 'css',
        name: 'CSS3',
        glow: '#1572B6',
        active: true,
        svg: `<svg viewBox="0 0 64 64" class="w-10 h-10"><rect width="64" height="64" rx="14" fill="#131f2c"/><polygon points="16,12 48,12 45,48 32,52 19,48" fill="#1572B6"/><polygon points="32,15 44.8,15 42.3,45.5 32,48.5" fill="#33A9DC"/><polygon points="32,23 42,23 41.2,34 32,34 32,29.5 37,29.5 37.3,27 32,27" fill="#fff"/><polygon points="32,39.5 27.5,38.2 27.2,35.5 23,35.5 23.6,41.8 32,44.2" fill="#ebebeb"/><polygon points="32,23 22,23 22.4,27 32,27" fill="#ebebeb"/><polygon points="32,29.5 23.2,29.5 23.6,34 32,34" fill="#ebebeb"/><polygon points="32,39.5 36.5,38.2 37,34 32,34 32,44.2 40.2,41.8 41.2,29.5 32,29.5" fill="#fff"/></svg>`
      },
      {
        id: 'git',
        name: 'Git',
        glow: '#F05032',
        active: true,
        svg: `<svg viewBox="0 0 64 64" class="w-10 h-10"><rect width="64" height="64" rx="14" fill="#261816"/><path d="M51.5 29.5l-17-17a3.5 3.5 0 00-5 0l-3.6 3.6 4.6 4.6a4.2 4.2 0 015.3 5.3l4.4 4.4a4.2 4.2 0 11-2.5 2.5L33.5 28.7v11a4.2 4.2 0 11-3.5 0V28.3a4.2 4.2 0 01-2.3-5.5L23.2 18.3l-10.7 10.7a3.5 3.5 0 000 5l17 17a3.5 3.5 0 005 0l17-17a3.5 3.5 0 000-5z" fill="#F05032"/></svg>`
      },
      {
        id: 'github',
        name: 'GitHub',
        glow: '#a855f7',
        active: true,
        svg: `<svg viewBox="0 0 64 64" class="w-10 h-10"><rect width="64" height="64" rx="14" fill="#161b22"/><path fill-rule="evenodd" clip-rule="evenodd" d="M32 12c-11 0-20 9-20 20 0 8.9 5.7 16.4 13.7 19 .9.2 1.3-.4 1.3-.9v-3.4c-5.6 1.2-6.7-2.7-6.7-2.7-.9-2.3-2.2-2.9-2.2-2.9-1.8-1.2.1-1.2.1-1.2 2 .1 3.1 2.1 3.1 2.1 1.8 3.1 4.7 2.2 5.8 1.7.2-1.3.7-2.2 1.3-2.7-4.4-.5-9.1-2.2-9.1-9.9 0-2.2.8-4 2.1-5.4-.2-.5-.9-2.5.2-5.3 0 0 1.7-.5 5.5 2.1 1.6-.4 3.3-.7 5-.7s3.4.2 5 .7c3.8-2.6 5.5-2.1 5.5-2.1 1.1 2.8.4 4.8.2 5.3 1.3 1.4 2.1 3.2 2.1 5.4 0 7.7-4.7 9.4-9.1 9.9.7.6 1.4 1.8 1.4 3.7v5.5c0 .5.4 1.1 1.4.9C46.3 48.4 52 40.9 52 32c0-11-9-20-20-20z" fill="#f0f6fc"/></svg>`
      },
      {
        id: 'docker',
        name: 'Docker',
        glow: '#2496ED',
        active: true,
        svg: `<svg viewBox="0 0 64 64" class="w-10 h-10"><rect width="64" height="64" rx="14" fill="#122334"/><g fill="#2496ED"><rect x="16" y="27" width="6" height="5.5" rx="1"/><rect x="23" y="27" width="6" height="5.5" rx="1"/><rect x="30" y="27" width="6" height="5.5" rx="1"/><rect x="37" y="27" width="6" height="5.5" rx="1"/><rect x="23" y="20.5" width="6" height="5.5" rx="1"/><rect x="30" y="20.5" width="6" height="5.5" rx="1"/><rect x="30" y="14" width="6" height="5.5" rx="1"/><path d="M52.5 31.5c-1.3-.9-4.2-1.2-6.3-.7-.3-2.3-1.6-4.3-3.9-6l-1.3-.9-.9 1.3c-1.1 1.7-1.5 4.4-.2 6.5-.9.5-2.7 1.1-5.1 1.1H11.5c-.6 3.6.4 8.3 3.2 11.6 2.7 3.2 6.8 4.8 12.2 4.8 11.6 0 20.2-5.3 24.2-15.1 1.6.1 5 .1 6.8-3.3l-5.4.7z"/></g></svg>`
      },
      {
        id: 'nginx',
        name: 'Nginx',
        glow: '#009639',
        active: true,
        svg: `<svg viewBox="0 0 64 64" class="w-10 h-10"><rect width="64" height="64" rx="14" fill="#11261b"/><polygon points="32,10 51,21 51,43 32,54 13,43 13,21" fill="#009639"/><path d="M23 41V23h3.8l10.4 12.5V23H41v18h-3.8L26.8 28.5V41H23z" fill="#fff"/></svg>`
      },
      {
        id: 'cloudflare',
        name: 'Cloudflare',
        glow: '#F38020',
        active: true,
        svg: `<svg viewBox="0 0 64 64" class="w-10 h-10"><rect width="64" height="64" rx="14" fill="#271c13"/><path d="M43.5 39.5H18.2a6.8 6.8 0 01-.8-13.5 9.8 9.8 0 0119-2.8 7.5 7.5 0 017.1 16.3z" fill="#F38020"/><path d="M47.8 30.2a6 6 0 00-4.2 1.7 6.3 6.3 0 011.2 3.7v1.2h6.8a4.5 4.5 0 00-3.8-6.6z" fill="#FAAE40"/></svg>`
      },
      {
        id: 'vscode',
        name: 'VS Code',
        glow: '#007ACC',
        active: true,
        svg: `<svg viewBox="0 0 64 64" class="w-10 h-10"><rect width="64" height="64" rx="14" fill="#13202e"/><path d="M44.5 13l-18 16.5-10.5-8L12 24l10.5 8L12 40l4 2.5 10.5-8L44.5 51l7.5-3.7V16.7L44.5 13zm0 10.5v17L32 32l12.5-8.5z" fill="#007ACC"/><path d="M44.5 13l7.5 3.7v30.6L44.5 51V13z" fill="#1F9CF0"/></svg>`
      },
      {
        id: 'kali',
        name: 'Kali Linux',
        glow: '#268BEE',
        active: false,
        svg: `<svg viewBox="0 0 64 64" class="w-10 h-10"><rect width="64" height="64" rx="14" fill="#0f1c2e"/><path d="M32 11L49 19v13c0 11.5-7.4 20.5-17 24-9.6-3.5-17-12.5-17-24V19l17-8z" fill="#1d4ed8" fill-opacity="0.3" stroke="#38bdf8" stroke-width="2"/><path d="M24 35c3-8 8-12 16-14-4 5-5 9-3 14 2 4 0 8-5 10 1-4-1-7-8-10z" fill="#38bdf8"/></svg>`
      },
      {
        id: 'go',
        name: 'Golang',
        glow: '#00ADD8',
        active: false,
        svg: `<svg viewBox="0 0 64 64" class="w-10 h-10"><rect width="64" height="64" rx="14" fill="#11252d"/><text x="32" y="39" text-anchor="middle" fill="#00ADD8" font-family="Fira Code, monospace" font-weight="800" font-size="24">GO</text><line x1="12" y1="26" x2="20" y2="26" stroke="#00ADD8" stroke-width="2.5" stroke-linecap="round"/><line x1="10" y1="32" x2="18" y2="32" stroke="#00ADD8" stroke-width="2.5" stroke-linecap="round"/></svg>`
      },
      {
        id: 'php',
        name: 'PHP',
        glow: '#777BB4',
        active: false,
        svg: `<svg viewBox="0 0 64 64" class="w-10 h-10"><rect width="64" height="64" rx="14" fill="#1d1e2c"/><ellipse cx="32" cy="32" rx="22" ry="13" fill="#777BB4"/><text x="32" y="36" text-anchor="middle" fill="#fff" font-family="Inter, sans-serif" font-style="italic" font-weight="800" font-size="14">php</text></svg>`
      },
      {
        id: 'cpp',
        name: 'C++',
        glow: '#00599C',
        active: false,
        svg: `<svg viewBox="0 0 64 64" class="w-10 h-10"><rect width="64" height="64" rx="14" fill="#121e2b"/><polygon points="32,10 51,21 51,43 32,54 13,43 13,21" fill="#00599C"/><text x="32" y="37" text-anchor="middle" fill="#fff" font-family="Inter, sans-serif" font-weight="800" font-size="16">C++</text></svg>`
      },
      {
        id: 'mysql',
        name: 'MySQL',
        glow: '#4479A1',
        active: false,
        svg: `<svg viewBox="0 0 64 64" class="w-10 h-10"><rect width="64" height="64" rx="14" fill="#14222e"/><ellipse cx="32" cy="20" rx="14" ry="5" fill="#4479A1"/><path d="M18 20v12c0 2.8 6.3 5 14 5s14-2.2 14-5V20c0 2.8-6.3 5-14 5s-14-2.2-14-5z" fill="#38bdf8" fill-opacity="0.7"/><path d="M18 32v12c0 2.8 6.3 5 14 5s14-2.2 14-5V32c0 2.8-6.3 5-14 5s-14-2.2-14-5z" fill="#f59e0b" fill-opacity="0.85"/></svg>`
      }
    ];

    let currentTheme = 'tokyonight';

    const themes = {
      tokyonight: {
        bg: '#1a1b27',
        border: '#2f334d',
        title: '#70a5fd',
        text: '#38bdae',
        ring: '#bf91f3',
        typingHex: '00F7FF'
      },
      radical: {
        bg: '#141321',
        border: '#381c3a',
        title: '#fe428e',
        text: '#a9fef7',
        ring: '#f8d847',
        typingHex: 'FE428E'
      },
      dracula: {
        bg: '#282a36',
        border: '#44475a',
        title: '#ff6e96',
        text: '#f8f8f2',
        ring: '#bd93f9',
        typingHex: 'BD93F9'
      },
      cyberpunk: {
        bg: '#0b0c10',
        border: '#00f7ff',
        title: '#fcee09',
        text: '#00f7ff',
        ring: '#ff003c',
        typingHex: 'FCEE09'
      }
    };

    function renderSkills() {
      const grid = document.getElementById('techStackGrid');
      const checkboxes = document.getElementById('skillCheckboxes');
      grid.innerHTML = '';
      checkboxes.innerHTML = '';

      allSkills.forEach((skill, index) => {
        // Render checkbox in customizer
        const btn = document.createElement('button');
        btn.className = `px-2.5 py-1 rounded-lg border text-xs font-medium transition flex items-center gap-1.5 ${
          skill.active
            ? 'bg-cyan-500/20 border-cyan-500 text-cyan-300'
            : 'bg-[#161b22] border-[#30363d] text-[#8b949e] hover:text-white'
        }`;
        btn.innerHTML = `<span>${skill.active ? '✓' : '+'}</span> <span>${skill.name}</span>`;
        btn.onclick = () => {
          allSkills[index].active = !allSkills[index].active;
          renderSkills();
          updateRawMarkdown();
        };
        checkboxes.appendChild(btn);

        // Render High-Graphics 3D Squircle Card in Preview
        if (skill.active) {
          const iconCard = document.createElement('div');
          iconCard.className = 'group relative flex flex-col items-center justify-center p-2.5 rounded-2xl bg-[#0d1117] border border-[#30363d] hover:border-cyan-400/60 shadow-lg transition-all duration-300 transform hover:-translate-y-1.5 hover:scale-105 cursor-pointer select-none w-[74px]';
          iconCard.style.boxShadow = `0 8px 20px -6px ${skill.glow}25`;
          iconCard.innerHTML = `
            <div class="relative flex items-center justify-center rounded-xl overflow-hidden shadow-md ring-1 ring-white/10 group-hover:ring-white/25 transition">
              ${skill.svg}
              <div class="absolute inset-0 bg-gradient-to-tr from-transparent via-white/5 to-white/15 pointer-events-none"></div>
            </div>
            <span class="text-[10px] font-semibold text-[#c9d1d9] group-hover:text-white mt-1.5 tracking-tight truncate max-w-[66px]">${skill.name}</span>
          `;
          grid.appendChild(iconCard);
        }
      });
    }

    function changeTheme(themeKey) {
      currentTheme = themeKey;
      const t = themes[themeKey];

      // Update Typing, Banner Accent & Counter Color
      document.getElementById('typingText').style.color = `#${t.typingHex}`;
      document.getElementById('typingCursor').style.backgroundColor = `#${t.typingHex}`;
      document.getElementById('viewsBadgeColor').style.backgroundColor = `#${t.typingHex}`;
      const bannerAccent = document.getElementById('bannerAccentText');
      if (bannerAccent) bannerAccent.setAttribute('fill', `#${t.typingHex}`);

      updateRawMarkdown();
    }

    // 3. Viewport Switcher (Desktop vs Mobile)
    function setViewport(mode) {
      const frame = document.getElementById('previewFrame');
      const grid = document.getElementById('profileGrid');
      const sidebar = document.getElementById('profileSidebar');
      const readmeCol = document.getElementById('readmeColumn');
      const avatarGroup = document.getElementById('avatarGroup');
      const btnDesktop = document.getElementById('btnDesktop');
      const btnMobile = document.getElementById('btnMobile');

      if (mode === 'mobile') {
        frame.className = 'mobile-frame gh-ltr';
        grid.className = 'bg-[#0d1117] p-4 flex flex-col gap-6';
        sidebar.className = 'w-full flex flex-col gap-3';
        readmeCol.className = 'w-full';
        avatarGroup.className = 'flex flex-row items-center gap-4';

        btnMobile.className = 'px-2.5 py-1.5 rounded-md font-medium transition flex items-center gap-1.5 bg-[#21262d] text-white shadow-sm';
        btnDesktop.className = 'px-2.5 py-1.5 rounded-md font-medium transition flex items-center gap-1.5 text-[#8b949e] hover:text-white';
      } else {
        frame.className = 'desktop-frame gh-ltr';
        grid.className = 'bg-[#0d1117] border-x border-b border-[#30363d] rounded-b-xl p-4 sm:p-6 grid grid-cols-1 lg:grid-cols-12 gap-6';
        sidebar.className = 'lg:col-span-3 flex flex-col gap-4';
        readmeCol.className = 'lg:col-span-9';
        avatarGroup.className = 'flex sm:flex-row lg:flex-col items-center sm:items-start gap-4';

        btnDesktop.className = 'px-2.5 py-1.5 rounded-md font-medium transition flex items-center gap-1.5 bg-[#21262d] text-white shadow-sm';
        btnMobile.className = 'px-2.5 py-1.5 rounded-md font-medium transition flex items-center gap-1.5 text-[#8b949e] hover:text-white';
      }
    }

    // 4. Generate Dynamic Markdown Output
    function generateMarkdownString() {
      const activeIds = allSkills.filter(s => s.active).map(s => s.id).join(',');
      const t = themes[currentTheme];

      return `<div align="center">

  <!-- Animated Cyber Hero Banner -->
  <img width="100%" src="https://capsule-render.vercel.app/api?type=waving&height=210&color=0:0d1117,50:111c35,100:${t.typingHex.toLowerCase()}&text=Saeed%20Salari%20(SSLRI)&fontColor=ffffff&fontSize=42&fontAlignY=38&desc=%F0%9F%9B%A1%EF%B8%8F%20Co-Founder%20%26%20CEO%20at%20Iran%20YouSec%20%20%E2%80%A2%20%20%E2%9A%A1%20Cybersecurity%20%26%20Automation&descAlignY=62&descSize=16&animation=fadeIn" alt="SSLRI Banner" />

  <!-- Animated Typing Header -->
  <a href="https://github.com/SSLRI">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&duration=3000&pause=1000&color=${t.typingHex}&center=true&vCenter=true&width=650&lines=Hi+there+%F0%9F%91%8B%2C+I'm+Saeed+Salari+(SSLRI);Co-Founder+%26+CEO+of+Iran+YouSec;Cybersecurity+Enthusiast+%26+Tech+Explorer;Automation+%26+Linux+Administration" alt="Typing SVG" />
  </a>

  <!-- Modern Dark-Label Social & Views Badges -->
  <p align="center">
    <a href="https://www.sslri.ir" target="_blank">
      <img src="https://img.shields.io/badge/Website-sslri.ir-0A66C2?style=for-the-badge&logo=googlechrome&logoColor=0A66C2&labelColor=161b22" alt="Website" />
    </a>
    <a href="https://t.me/sslri" target="_blank">
      <img src="https://img.shields.io/badge/Telegram-@sslri-26A5E4?style=for-the-badge&logo=telegram&logoColor=26A5E4&labelColor=161b22" alt="Telegram" />
    </a>
    <a href="https://instagram.com/sslri" target="_blank">
      <img src="https://img.shields.io/badge/Instagram-@sslri-E4405F?style=for-the-badge&logo=instagram&logoColor=E4405F&labelColor=161b22" alt="Instagram" />
    </a>
    <img src="https://komarev.com/ghpvc/?username=SSLRI&label=VIEWS&color=${t.typingHex.toLowerCase()}&style=for-the-badge" alt="SSLRI Profile Views" />
  </p>

</div>

---

### 👨‍💻 About Me

<img align="right" src="./dev.gif" width="280" alt="Coding Animation" />

- 🛡️ **Co-Founder & CEO** at **Iran YouSec**
- 🔍 Curious mind exploring the depths of **Cybersecurity**, **Network Security**, and **Technology**
- ⚙️ Experienced in **Linux Server Administration**, **Bash Scripting**, and **Task Automation**
- 🤖 Building smart **Telegram Bots**, CLI tools, and security utilities
- 🌐 Portfolio & Updates: **[sslri.ir](https://www.sslri.ir)**

<br clear="right"/>

---

### 🛠️ Tech Stack & Cyber Arsenal

<div align="center">
  <a href="https://github.com/SSLRI">
    <img src="https://skillicons.dev/icons?i=${activeIds}&theme=dark&perline=6" alt="Tech Stack" />
  </a>
</div>

---

<div align="center">
  <sub>⚡ <i>"Security is not a product, but a process."</i></sub>
</div>`;
    }

    function updateRawMarkdown() {
      document.getElementById('rawMarkdownOutput').textContent = generateMarkdownString();
    }
// ... existing code ... -->
```
