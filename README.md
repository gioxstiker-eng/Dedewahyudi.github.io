[portfolio (4).html](https://github.com/user-attachments/files/34723790/portfolio.4.html)
<!DOCTYPE html>
<html lang="id" class="scroll-smooth">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Dede Wahyudi — Jasa Desain Grafis</title>
  <meta name="description" content="Jasa desain logo, undangan, banner, dan company profile oleh Dede Wahyudi." />
  <meta name="theme-color" content="#050505" />
  <link rel="icon" href="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 64 64'%3E%3Cdefs%3E%3ClinearGradient id='g' x1='0' y1='0' x2='1' y2='1'%3E%3Cstop offset='0' stop-color='%23FF1F3D'/%3E%3Cstop offset='1' stop-color='%23FF8A95'/%3E%3C/linearGradient%3E%3C/defs%3E%3Crect width='64' height='64' rx='16' fill='%23000000'/%3E%3Ctext x='32' y='42' font-family='Arial,sans-serif' font-size='26' font-weight='900' font-style='italic' text-anchor='middle' fill='url(%23g)'%3EDW%3C/text%3E%3C/svg%3E" />
  <script src="https://cdn.tailwindcss.com"></script>
  <script>
    if (window.tailwind) tailwind.config = { theme: { extend: { fontFamily: { sans: ['Inter', 'ui-sans-serif', 'system-ui', 'sans-serif'] } } } };
  </script>
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link href="https://fonts.googleapis.com/css2?family=Inter:ital,wght@0,400;0,500;0,600;0,700;0,800;1,500;1,700;1,800&display=swap" rel="stylesheet" />
  <style>
    html { scroll-behavior: smooth; }
    section[id] { scroll-margin-top: calc(var(--hh, 200px) + 8px); }
    .no-scrollbar { scrollbar-width: none; }
    .no-scrollbar::-webkit-scrollbar { display: none; }
    .tab { transition: background .2s, color .2s, border-color .2s; border-color: transparent; color: rgba(255,255,255,.72); }
    .tab.active { border-color: rgba(255,31,61,.6); background: rgba(255,31,61,.1); color: #ff6b7a; }
    .chip { border: 1px solid rgba(255,255,255,.15); border-radius: 9999px; padding: .55rem 1.1rem; font-size: .9rem; font-weight: 500; color: rgba(255,255,255,.75); transition: all .2s; white-space: nowrap; }
    .chip:hover { border-color: rgba(255,31,61,.6); color: #fff; }
    .chip.active { border-color: transparent; background: linear-gradient(90deg, #FF1F3D, #000000); color: #fff; font-weight: 700; }
    .grad-btn { background: linear-gradient(90deg, #FF1F3D, #000000); color: #fff; box-shadow: 0 0 32px rgba(255,31,61,.3); transition: transform .2s, box-shadow .2s; }
    .grad-btn:hover { transform: translateY(-2px); box-shadow: 0 0 44px rgba(255,31,61,.45); }
    .card svg, .gal svg { transition: transform .5s; }
    .card:hover svg, .gal:hover svg { transform: scale(1.05); }

    .reveal { opacity: 0; transform: translateY(18px); transition: opacity .7s ease, transform .7s ease; }
    .reveal.show { opacity: 1; transform: none; }

    /* Cara kerja */
    .step { opacity: 0; transform: translateY(24px); }
    .step-dot { transform: scale(.6); }
    .step-icon path, .step-icon circle { stroke-dasharray: 1; stroke-dashoffset: 1; }
    .step-line-h { width: 0; }
    .conn-v { position: absolute; left: 2rem; top: 2rem; width: 2px; height: calc(100% + 2.5rem); transform: translateX(-50%); background: rgba(255,255,255,.1); }
    .conn-v::after { content: ''; position: absolute; inset: 0; background: linear-gradient(#FF1F3D, #000000); transform: scaleY(0); transform-origin: top; }
    .steps-play .step { animation: stepIn .6s ease forwards; animation-delay: calc(var(--i) * .6s); }
    .steps-play .step-dot { animation: dotPop .6s ease forwards, ring 1.2s ease-out 2; animation-delay: calc(var(--i) * .6s + .1s), calc(var(--i) * .6s + .6s); }
    .steps-play .step-icon path, .steps-play .step-icon circle { animation: draw .9s ease forwards; animation-delay: calc(var(--i) * .6s + .45s); }
    .steps-play .step-line-h { width: 100%; transition: width 1.8s linear .1s; }
    .steps-play .conn-v::after { animation: grow .6s linear forwards; animation-delay: calc(var(--i) * .6s + .3s); }
    @keyframes stepIn { to { opacity: 1; transform: none; } }
    @keyframes dotPop { 0% { transform: scale(.6); } 60% { transform: scale(1.15); } 100% { transform: scale(1); } }
    @keyframes ring { 0% { box-shadow: 0 0 0 0 rgba(255,31,61,.5); } 100% { box-shadow: 0 0 0 16px rgba(255,31,61,0); } }
    @keyframes draw { to { stroke-dashoffset: 0; } }
    @keyframes grow { to { transform: scaleY(1); } }
    @keyframes floaty { 0%,100% { transform: translateY(0); } 50% { transform: translateY(-10px); } }
    .floaty { animation: floaty 6s ease-in-out infinite; }
    @media (prefers-reduced-motion: reduce) {
      html { scroll-behavior: auto; }
      .reveal, .step { opacity: 1; transform: none; }
      .step-dot { transform: none; }
      .step-icon path, .step-icon circle { stroke-dashoffset: 0; }
      .step-line-h { width: 100%; }
      .conn-v::after { transform: none; }
      .steps-play .step, .steps-play .step-dot, .steps-play .step-icon path, .steps-play .step-icon circle, .steps-play .conn-v::after, .floaty { animation: none; }
      .card svg, .gal svg { transition: none; }
    }
    ::selection { background: #FF1F3D; color: #fff; }
  </style>
</head>
<body class="bg-[#050505] pb-8 font-sans text-white/80 antialiased">

  <!-- Logo DW (dipakai berulang) -->
  <svg width="0" height="0" class="absolute" aria-hidden="true" focusable="false">
    <defs>
      <linearGradient id="gDW" x1="0" y1="0" x2="1" y2="1">
        <stop offset="0" stop-color="#FF1F3D"/><stop offset="1" stop-color="#FF8A95"/>
      </linearGradient>
    </defs>
    <symbol id="logoDW" viewBox="0 0 64 64">
      <rect width="64" height="64" rx="16" fill="#000000"/>
      <rect x="1.5" y="1.5" width="61" height="61" rx="14.5" fill="none" stroke="url(#gDW)" stroke-width="1.5" opacity=".7"/>
      <text x="32" y="42" text-anchor="middle" font-family="Inter,Arial,sans-serif" font-style="italic" font-weight="900" font-size="26" fill="url(#gDW)">DW</text>
    </symbol>
  </svg>

  <!-- HEADER -->
  <header id="topbar" class="sticky top-0 z-50 border-b border-white/10 bg-[#050505]/90 backdrop-blur-xl">
    <div class="mx-auto max-w-6xl px-5">
      <div class="flex items-center gap-3 py-3">
        <a href="#home" class="flex shrink-0 items-center gap-2" aria-label="Dede Wahyudi — beranda">
          <svg class="h-10 w-10 rounded-xl shadow-[0_0_18px_rgba(255,31,61,.25)]" aria-hidden="true"><use href="#logoDW"/></svg>
          <span class="text-base font-medium italic text-white">Dede <span class="text-[#ff4d5e]">Wahyudi</span></span>
        </a>

        <form id="searchForm" class="flex min-w-0 flex-1 items-center gap-2" role="search">
          <label class="relative min-w-0 flex-1">
            <span class="sr-only">Cari desain</span>
            <svg class="pointer-events-none absolute left-3.5 top-1/2 h-5 w-5 -translate-y-1/2 text-white/50" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" viewBox="0 0 24 24"><circle cx="11" cy="11" r="7"/><path d="M20 20l-3.5-3.5"/></svg>
            <input id="q" type="search" placeholder="Cari desain..." autocomplete="off" class="h-10 w-full rounded-full border border-white/15 bg-white/5 pl-10 pr-4 text-sm text-white outline-none placeholder:text-white/40 focus:border-[#ff1f3d]/70 focus:ring-2 focus:ring-[#ff1f3d]/30" />
          </label>
          <button type="submit" aria-label="Cari" class="grad-btn flex h-10 w-10 shrink-0 items-center justify-center rounded-full text-sm font-semibold sm:w-auto sm:px-6">
            <svg class="h-5 w-5 sm:hidden" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" viewBox="0 0 24 24" aria-hidden="true"><circle cx="11" cy="11" r="7"/><path d="M20 20l-3.5-3.5"/></svg>
            <span class="hidden sm:inline">Cari</span>
          </button>
        </form>
      </div>

      <nav id="tabs" aria-label="Menu" class="no-scrollbar -mx-5 flex gap-2 overflow-x-auto px-5 pb-3">
        <a href="#home" class="tab shrink-0 rounded-full border px-5 py-2.5 text-base font-medium">Home</a>
        <a href="#unggulan" class="tab shrink-0 rounded-full border px-5 py-2.5 text-base font-medium">Unggulan</a>
        <a href="#katalog" class="tab shrink-0 rounded-full border px-5 py-2.5 text-base font-medium">Katalog</a>
        <a href="#galeri" class="tab shrink-0 rounded-full border px-5 py-2.5 text-base font-medium">Galeri</a>
        <a href="#cara-kerja" class="tab shrink-0 rounded-full border px-5 py-2.5 text-base font-medium">Cara Kerja</a>
        <a href="#tentang" class="tab shrink-0 rounded-full border px-5 py-2.5 text-base font-medium">Tentang</a>
        <a href="#kontak" class="tab shrink-0 rounded-full border px-5 py-2.5 text-base font-medium">Kontak</a>
      </nav>
    </div>
  </header>

  <main>
    <!-- HOME -->
    <section id="home" class="relative overflow-hidden">
      <div class="pointer-events-none absolute inset-0 bg-[radial-gradient(ellipse_at_20%_10%,rgba(255,31,61,.45),transparent_60%),radial-gradient(ellipse_at_95%_20%,rgba(255,31,61,.28),transparent_55%)]"></div>
      <div class="relative mx-auto grid max-w-6xl items-center gap-10 px-5 pb-16 pt-14 md:grid-cols-[1.3fr_1fr]">
        <div>
          <div class="reveal flex items-center gap-5">
            <svg class="h-24 w-24 shrink-0 rounded-3xl shadow-[0_0_40px_rgba(255,31,61,.25)]" aria-hidden="true"><use href="#logoDW"/></svg>
            <div>
              <p class="text-lg font-semibold uppercase tracking-[.25em] text-white">Jasa Desain Grafis</p>
              <p class="mt-1 text-sm font-semibold uppercase tracking-[.2em] text-[#ff6b7a]">Logo • Undangan • Banner • Compro</p>
            </div>
          </div>

          <h1 class="reveal mt-10 text-5xl font-extrabold italic leading-[1.05] tracking-tight text-white sm:text-6xl lg:text-7xl">
            Desain Yang<br />
            <span class="bg-gradient-to-r from-[#ff6b7a] to-[#ff1f3d] bg-clip-text text-transparent">Bicara.</span><br />
            Brand Yang<br />
            <span class="bg-gradient-to-r from-white to-zinc-400 bg-clip-text pr-2 text-transparent">Diingat.</span>
          </h1>

          <p class="reveal mt-8 max-w-xl text-xl leading-relaxed text-white/60">
            Halo, saya Dede Wahyudi. Saya membuat logo, undangan, banner, dan company profile yang rapi, fungsional, dan siap cetak.
          </p>

          <div class="reveal mt-10 flex flex-wrap gap-4">
            <a href="#katalog" class="grad-btn inline-flex items-center gap-3 rounded-full px-8 py-4 text-lg font-semibold">
              Lihat Katalog
              <svg class="h-5 w-5" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round" viewBox="0 0 24 24"><path d="M5 12h14M13 6l6 6-6 6"/></svg>
            </a>
          </div>
        </div>

        <div class="reveal relative hidden items-center justify-center md:flex" aria-hidden="true">
          <div class="absolute h-72 w-72 rounded-full bg-[#ff1f3d]/20 blur-3xl"></div>
          <div class="absolute -right-4 top-6 h-48 w-48 rounded-full bg-[#ff1f3d]/10 blur-3xl"></div>
          <svg class="floaty relative h-64 w-64 rounded-[2.5rem] shadow-[0_0_80px_rgba(255,31,61,.3)] lg:h-72 lg:w-72"><use href="#logoDW"/></svg>
        </div>
      </div>
    </section>

    <!-- Chip & statistik -->
    <div class="mx-auto max-w-6xl px-5">
      <div class="reveal flex flex-wrap gap-3">
        <span class="rounded-full border border-white/10 bg-white/5 px-6 py-3 text-sm font-semibold uppercase text-white">Desain Orisinal</span>
        <span class="rounded-full border border-white/10 bg-white/5 px-6 py-3 text-sm font-semibold uppercase text-white">Siap Cetak</span>
        <span class="rounded-full border border-white/10 bg-white/5 px-6 py-3 text-sm font-semibold uppercase text-white">Revisi</span>
      </div>

      <dl class="reveal mt-10 grid grid-cols-3 divide-x divide-white/10 text-left">
        <div class="pr-4"><dd class="text-4xl font-semibold tabular-nums text-white"><span class="counter" data-target="5">5</span>+</dd><dt class="mt-1 text-sm text-white/50">Tahun pengalaman</dt></div>
        <div class="px-4"><dd class="text-4xl font-semibold tabular-nums text-white"><span class="counter" data-target="40">40</span>+</dd><dt class="mt-1 text-sm text-white/50">Proyek selesai</dt></div>
        <div class="pl-4"><dd class="text-4xl font-semibold tabular-nums text-white"><span class="counter" data-target="25">25</span>+</dd><dt class="mt-1 text-sm text-white/50">Klien dilayani</dt></div>
      </dl>
    </div>

    <!-- UNGGULAN -->
    <section id="unggulan" class="mx-auto max-w-6xl px-5 pt-16">
      <div class="reveal overflow-hidden rounded-[2rem] border border-[#ff1f3d]/20 bg-gradient-to-b from-[#3a0b12]/70 to-[#0b0b0c] p-5 shadow-[0_0_60px_rgba(255,31,61,.08)] sm:p-7">
        <div class="flex items-center justify-between gap-3">
          <p id="featLabel" class="text-sm font-semibold uppercase tracking-[.25em] text-[#ff6b7a]">Karya Pilihan • 1 / 6</p>
          <button id="featPause" type="button" class="flex items-center gap-2 rounded-full border border-white/15 bg-white/5 px-5 py-2.5 text-sm font-semibold text-white transition hover:border-[#ff1f3d]/60">
            <svg id="icoPause" class="h-4 w-4" fill="currentColor" viewBox="0 0 24 24"><rect x="5" y="4" width="5" height="16" rx="1.5"/><rect x="14" y="4" width="5" height="16" rx="1.5"/></svg>
            <svg id="icoPlay" class="hidden h-4 w-4" fill="currentColor" viewBox="0 0 24 24"><path d="M7 4.5v15a1 1 0 0 0 1.5.9l12-7.5a1 1 0 0 0 0-1.8l-12-7.5A1 1 0 0 0 7 4.5z"/></svg>
            <span id="featPauseText">Jeda</span>
          </button>
        </div>
        <div class="mt-4 h-1.5 overflow-hidden rounded-full bg-white/10"><div id="featBar" class="h-full w-0 rounded-full bg-gradient-to-r from-[#ff1f3d] to-black"></div></div>
        <p id="featCount" class="mt-2 text-right text-sm text-white/50">&nbsp;</p>

        <div class="mt-4 grid gap-6 md:grid-cols-2 md:items-center">
          <button id="featMedia" type="button" class="relative block aspect-[4/3] w-full overflow-hidden rounded-3xl bg-[#0c0c0d] text-left" aria-label="Lihat detail karya pilihan">
            <span class="absolute left-4 top-4 z-10 rounded-full bg-black/80 px-4 py-2 text-sm font-semibold uppercase text-white">Rekomendasi</span>
            <span id="featSvg" class="block h-full w-full"></span>
          </button>
          <div>
            <p id="featCat" class="text-sm font-semibold uppercase tracking-[.2em] text-[#ff6b7a]"></p>
            <h2 id="featTitle" class="mt-2 text-3xl font-semibold text-white sm:text-4xl"></h2>
            <p id="featDesc" class="mt-3 leading-relaxed text-white/60"></p>
            <p id="featPrice" class="mt-4 text-2xl font-bold text-[#ff4d5e]"></p>
            <div class="mt-6 flex flex-wrap items-center gap-3">
              <button id="featAdd" type="button" class="grad-btn rounded-full px-6 py-3 font-semibold">Tambah ke Pesanan</button>
              <button id="featPrev" type="button" aria-label="Sebelumnya" class="flex h-12 w-12 items-center justify-center rounded-full border border-white/15 text-white transition hover:border-[#ff1f3d]/60"><svg class="h-5 w-5" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round" viewBox="0 0 24 24"><path d="M15 5l-7 7 7 7"/></svg></button>
              <button id="featNext" type="button" aria-label="Berikutnya" class="flex h-12 w-12 items-center justify-center rounded-full border border-white/15 text-white transition hover:border-[#ff1f3d]/60"><svg class="h-5 w-5" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round" viewBox="0 0 24 24"><path d="M9 5l7 7-7 7"/></svg></button>
            </div>
          </div>
        </div>
      </div>

      <!-- Banner promo -->
      <div class="mt-8 grid gap-5 md:grid-cols-2">
        <div class="reveal relative overflow-hidden rounded-3xl border border-[#ff1f3d]/20 bg-gradient-to-br from-[#1a0508] via-[#5c0b16] to-[#ff1f3d]/80 p-7">
          <div class="relative z-10 max-w-[60%]">
            <h3 class="text-3xl font-semibold text-white">Desain Eksklusif</h3>
            <p class="mt-3 leading-relaxed text-white/70">Dibuat khusus untuk kebutuhanmu, bukan template.</p>
            <a href="#katalog" class="mt-6 inline-flex items-center gap-2 rounded-full border border-white/20 bg-black/60 px-6 py-3 font-semibold text-white transition hover:border-[#ff1f3d]">Lihat Katalog <span aria-hidden="true">&rarr;</span></a>
          </div>
          <svg class="absolute -right-8 top-1/2 h-56 w-56 -translate-y-1/2" viewBox="0 0 200 200" aria-hidden="true">
            <circle cx="100" cy="100" r="96" fill="#000000"/>
            <g fill="none" stroke="#3a1218" stroke-width="1.5"><circle cx="100" cy="100" r="86"/><circle cx="100" cy="100" r="74"/><circle cx="100" cy="100" r="62"/><circle cx="100" cy="100" r="50"/></g>
            <circle cx="100" cy="100" r="30" fill="#FF1F3D"/><circle cx="100" cy="100" r="7" fill="#000000"/>
          </svg>
        </div>
        <div class="reveal relative overflow-hidden rounded-3xl border border-white/15 bg-gradient-to-br from-[#3a3a3c] via-[#161617] to-black p-7 text-right">
          <svg class="absolute -left-16 top-1/2 h-64 w-64 -translate-y-1/2" viewBox="0 0 200 200" fill="none" stroke="#ff6b7a" stroke-opacity=".55" stroke-width="1.5" aria-hidden="true">
            <circle cx="100" cy="100" r="96"/><circle cx="100" cy="100" r="60"/><path d="M4 100h192M100 4v192"/>
          </svg>
          <div class="relative z-10 ml-auto max-w-[70%]">
            <h3 class="text-3xl font-semibold text-white">Pesan Dari Mana Saja</h3>
            <p class="mt-3 leading-relaxed text-white/70">Kirim brief lewat WhatsApp, saya kerjakan secara online.</p>
            <a href="#kontak" class="mt-6 inline-flex items-center gap-2 rounded-full border border-white/20 bg-black/70 px-6 py-3 font-semibold text-white transition hover:border-white">Hubungi <span aria-hidden="true">&rarr;</span></a>
          </div>
        </div>
      </div>

      <!-- Desain unggulan -->
      <div class="mt-16 flex items-center justify-between gap-3">
        <h2 class="flex items-center gap-3 text-3xl font-medium text-white sm:text-4xl">
          <svg class="h-8 w-8 text-[#ff6b7a]" viewBox="0 0 24 24" fill="currentColor" aria-hidden="true"><path d="M12 2l2.2 6.3L21 10l-6.8 1.7L12 18l-2.2-6.3L3 10l6.8-1.7z"/></svg>
          Desain Unggulan
        </h2>
        <a href="#katalog" class="flex shrink-0 items-center gap-2 text-lg font-medium text-[#ff4d5e] hover:text-[#ff8a95]">Lihat Semua <span aria-hidden="true">&rarr;</span></a>
      </div>
      <div id="featGrid" class="mt-8 grid grid-cols-2 gap-4 lg:grid-cols-4"></div>
    </section>

    <!-- KATALOG -->
    <section id="katalog" class="mx-auto max-w-6xl px-5 pt-24">
      <div class="reveal">
        <p class="text-sm font-semibold uppercase tracking-[.25em] text-[#ff6b7a]">Katalog</p>
        <h2 class="mt-3 text-4xl font-semibold text-white sm:text-5xl">Semua Desain</h2>
        <p class="mt-3 max-w-xl text-white/60">Pilih desain yang kamu suka, ketuk untuk melihat detail, lalu tambahkan ke pesanan.</p>
      </div>

      <div class="no-scrollbar -mx-5 mt-8 flex gap-2 overflow-x-auto px-5 pb-1" id="chips" role="group" aria-label="Filter kategori">
          <button type="button" class="chip" data-cat="all">Semua</button>
          <button type="button" class="chip" data-cat="undangan">Undangan</button>
          <button type="button" class="chip" data-cat="banner">Banner</button>
          <button type="button" class="chip" data-cat="logo">Logo</button>
          <button type="button" class="chip" data-cat="compro">Company Profile</button>
      </div>
      <p id="resultCount" class="mt-4 text-sm text-white/50" aria-live="polite"></p>

      <div id="catalogGrid" class="mt-4 grid grid-cols-2 gap-4 md:grid-cols-3 lg:grid-cols-4">
          <article class="card group overflow-hidden rounded-3xl border border-white/10 bg-[#0f0f10] transition hover:-translate-y-1 hover:border-[#ff1f3d]/40 hover:shadow-[0_0_30px_rgba(255,31,61,.15)]" data-id="u1" data-cat="undangan" data-price="85000" data-title="Undangan Pernikahan" data-desc="Desain elegan dengan bingkai emas tipis dan tipografi klasik. Siap cetak dengan bleed dan ukuran jadi yang presisi." data-tags="Undangan · Pernikahan" data-search="undangan pernikahan undangan undangan · pernikahan desain elegan dengan bingkai emas tipis dan tipografi klasik. siap cetak dengan bleed dan ukuran jadi yang presisi.">
            <button type="button" class="open block aspect-[4/3] w-full overflow-hidden bg-[#0c0c0d] text-left focus-visible:outline focus-visible:outline-2 focus-visible:outline-[#ff1f3d]" aria-label="Lihat detail Undangan Pernikahan">
              <svg viewBox="0 0 400 260" class="h-full w-full transition duration-500 group-hover:scale-105" preserveAspectRatio="xMidYMid slice" role="img" aria-label="Contoh desain undangan pernikahan" xmlns="http://www.w3.org/2000/svg">
              <rect width="400" height="260" fill="#0A0A0A"/>
              <rect x="150" y="38" width="150" height="204" rx="6" fill="#FF1F3D" transform="rotate(8 225 140)"/>
              <rect x="125" y="28" width="150" height="204" rx="6" fill="#FFF5F5"/>
              <rect x="133" y="36" width="134" height="188" rx="3" fill="none" stroke="#FF1F3D" stroke-width="1.5"/>
              <circle cx="200" cy="82" r="20" fill="none" stroke="#FF1F3D" stroke-width="2"/>
              <circle cx="200" cy="82" r="8" fill="#FF1F3D"/>
              <rect x="165" y="124" width="70" height="6" rx="3.0" fill="#0A0A0A"/>
              <rect x="150" y="140" width="100" height="4" rx="2.0" fill="#0A0A0A" opacity="0.35"/>
              <rect x="158" y="152" width="84" height="4" rx="2.0" fill="#0A0A0A" opacity="0.35"/>
              <rect x="172" y="178" width="56" height="14" rx="7.0" fill="#FF1F3D"/>
            </svg>
            </button>
            <div class="p-4">
              <h3 class="text-lg font-semibold leading-snug text-white">Undangan Pernikahan</h3>
              <p class="mt-1 text-sm text-white/50">Undangan</p>
              <div class="mt-4 flex items-center justify-between gap-2">
                <p class="whitespace-nowrap text-[15px] font-bold text-[#ff4d5e]"><span class="block text-[11px] font-medium text-white/40">Mulai</span>Rp 85.000</p>
                <button type="button" data-add class="flex h-10 w-10 shrink-0 items-center justify-center rounded-xl border border-white/15 text-white transition hover:border-[#ff1f3d] hover:bg-[#ff1f3d]/10 hover:text-[#ff6b7a]" aria-label="Tambah Undangan Pernikahan ke pesanan">
                  <svg class="h-5 w-5" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" viewBox="0 0 24 24"><path d="M3 4h2l2.3 10.5a1 1 0 0 0 1 .8h8.6a1 1 0 0 0 1-.8L19 8H6.2"/><circle cx="9" cy="19.5" r="1.3"/><circle cx="17" cy="19.5" r="1.3"/></svg>
                </button>
              </div>
            </div>
          </article>

          <article class="card group overflow-hidden rounded-3xl border border-white/10 bg-[#0f0f10] transition hover:-translate-y-1 hover:border-[#ff1f3d]/40 hover:shadow-[0_0_30px_rgba(255,31,61,.15)]" data-id="u2" data-cat="undangan" data-price="65000" data-title="Undangan Ulang Tahun" data-desc="Desain ceria dengan balon dan warna cerah untuk pesta ulang tahun anak maupun dewasa." data-tags="Undangan · Ulang Tahun" data-search="undangan ulang tahun undangan undangan · ulang tahun desain ceria dengan balon dan warna cerah untuk pesta ulang tahun anak maupun dewasa.">
            <button type="button" class="open block aspect-[4/3] w-full overflow-hidden bg-[#0c0c0d] text-left focus-visible:outline focus-visible:outline-2 focus-visible:outline-[#ff1f3d]" aria-label="Lihat detail Undangan Ulang Tahun">
              <svg viewBox="0 0 400 260" class="h-full w-full transition duration-500 group-hover:scale-105" preserveAspectRatio="xMidYMid slice" role="img" aria-label="Contoh desain undangan ulang tahun" xmlns="http://www.w3.org/2000/svg">
              <rect width="400" height="260" fill="#FF1F3D"/>
              <circle cx="60" cy="50" r="8" fill="#0A0A0A"/><circle cx="340" cy="70" r="6" fill="#fff"/><circle cx="84" cy="200" r="6" fill="#fff"/>
              <circle cx="330" cy="206" r="9" fill="#0A0A0A"/><circle cx="44" cy="130" r="5" fill="#fff"/><circle cx="360" cy="140" r="5" fill="#0A0A0A"/>
              <rect x="120" y="26" width="160" height="208" rx="14" fill="#fff"/>
              <path d="M170 100Q200 135 200 140M200 88Q200 120 200 140M230 100Q200 135 200 140" stroke="#0A0A0A" stroke-width="2" fill="none"/>
              <ellipse cx="170" cy="78" rx="18" ry="22" fill="#FF1F3D"/>
              <ellipse cx="200" cy="66" rx="18" ry="22" fill="#0A0A0A"/>
              <ellipse cx="230" cy="78" rx="18" ry="22" fill="#FF1F3D"/>
              <rect x="160" y="154" width="80" height="8" rx="4.0" fill="#0A0A0A"/>
              <rect x="150" y="172" width="100" height="5" rx="2.5" fill="#0A0A0A" opacity="0.35"/>
              <rect x="162" y="184" width="76" height="5" rx="2.5" fill="#0A0A0A" opacity="0.35"/>
              <rect x="172" y="204" width="56" height="14" rx="7.0" fill="#FF1F3D"/>
            </svg>
            </button>
            <div class="p-4">
              <h3 class="text-lg font-semibold leading-snug text-white">Undangan Ulang Tahun</h3>
              <p class="mt-1 text-sm text-white/50">Undangan</p>
              <div class="mt-4 flex items-center justify-between gap-2">
                <p class="whitespace-nowrap text-[15px] font-bold text-[#ff4d5e]"><span class="block text-[11px] font-medium text-white/40">Mulai</span>Rp 65.000</p>
                <button type="button" data-add class="flex h-10 w-10 shrink-0 items-center justify-center rounded-xl border border-white/15 text-white transition hover:border-[#ff1f3d] hover:bg-[#ff1f3d]/10 hover:text-[#ff6b7a]" aria-label="Tambah Undangan Ulang Tahun ke pesanan">
                  <svg class="h-5 w-5" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" viewBox="0 0 24 24"><path d="M3 4h2l2.3 10.5a1 1 0 0 0 1 .8h8.6a1 1 0 0 0 1-.8L19 8H6.2"/><circle cx="9" cy="19.5" r="1.3"/><circle cx="17" cy="19.5" r="1.3"/></svg>
                </button>
              </div>
            </div>
          </article>

          <article class="card group overflow-hidden rounded-3xl border border-white/10 bg-[#0f0f10] transition hover:-translate-y-1 hover:border-[#ff1f3d]/40 hover:shadow-[0_0_30px_rgba(255,31,61,.15)]" data-id="u3" data-cat="undangan" data-price="60000" data-title="Undangan Syukuran" data-desc="Bentuk lengkung yang hangat dan sederhana untuk acara syukuran dan kumpul keluarga." data-tags="Undangan · Syukuran" data-search="undangan syukuran undangan undangan · syukuran bentuk lengkung yang hangat dan sederhana untuk acara syukuran dan kumpul keluarga.">
            <button type="button" class="open block aspect-[4/3] w-full overflow-hidden bg-[#0c0c0d] text-left focus-visible:outline focus-visible:outline-2 focus-visible:outline-[#ff1f3d]" aria-label="Lihat detail Undangan Syukuran">
              <svg viewBox="0 0 400 260" class="h-full w-full transition duration-500 group-hover:scale-105" preserveAspectRatio="xMidYMid slice" role="img" aria-label="Contoh desain undangan syukuran" xmlns="http://www.w3.org/2000/svg">
              <rect width="400" height="260" fill="#F5F5F5"/>
              <ellipse cx="96" cy="190" rx="16" ry="34" fill="#FF1F3D" opacity=".85" transform="rotate(-24 96 190)"/>
              <ellipse cx="304" cy="190" rx="16" ry="34" fill="#FF1F3D" opacity=".85" transform="rotate(24 304 190)"/>
              <path d="M120 238V112a80 80 0 0 1 160 0v126z" fill="#0A0A0A"/>
              <path d="M134 238V114a66 66 0 0 1 132 0v124z" fill="none" stroke="#FF1F3D" stroke-width="1.5"/>
              <circle cx="200" cy="106" r="14" fill="#FF1F3D"/>
              <rect x="170" y="142" width="60" height="6" rx="3.0" fill="#fff"/>
              <rect x="156" y="158" width="88" height="4" rx="2.0" fill="#fff" opacity="0.55"/>
              <rect x="164" y="170" width="72" height="4" rx="2.0" fill="#fff" opacity="0.55"/>
              <rect x="176" y="192" width="48" height="12" rx="6.0" fill="#FF1F3D"/>
            </svg>
            </button>
            <div class="p-4">
              <h3 class="text-lg font-semibold leading-snug text-white">Undangan Syukuran</h3>
              <p class="mt-1 text-sm text-white/50">Undangan</p>
              <div class="mt-4 flex items-center justify-between gap-2">
                <p class="whitespace-nowrap text-[15px] font-bold text-[#ff4d5e]"><span class="block text-[11px] font-medium text-white/40">Mulai</span>Rp 60.000</p>
                <button type="button" data-add class="flex h-10 w-10 shrink-0 items-center justify-center rounded-xl border border-white/15 text-white transition hover:border-[#ff1f3d] hover:bg-[#ff1f3d]/10 hover:text-[#ff6b7a]" aria-label="Tambah Undangan Syukuran ke pesanan">
                  <svg class="h-5 w-5" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" viewBox="0 0 24 24"><path d="M3 4h2l2.3 10.5a1 1 0 0 0 1 .8h8.6a1 1 0 0 0 1-.8L19 8H6.2"/><circle cx="9" cy="19.5" r="1.3"/><circle cx="17" cy="19.5" r="1.3"/></svg>
                </button>
              </div>
            </div>
          </article>

          <article class="card group overflow-hidden rounded-3xl border border-white/10 bg-[#0f0f10] transition hover:-translate-y-1 hover:border-[#ff1f3d]/40 hover:shadow-[0_0_30px_rgba(255,31,61,.15)]" data-id="u4" data-cat="undangan" data-price="90000" data-title="Undangan Seminar" data-desc="Undangan landscape yang rapi dan formal untuk seminar, rapat, dan acara perusahaan." data-tags="Undangan · Acara Resmi" data-search="undangan seminar undangan undangan · acara resmi undangan landscape yang rapi dan formal untuk seminar, rapat, dan acara perusahaan.">
            <button type="button" class="open block aspect-[4/3] w-full overflow-hidden bg-[#0c0c0d] text-left focus-visible:outline focus-visible:outline-2 focus-visible:outline-[#ff1f3d]" aria-label="Lihat detail Undangan Seminar">
              <svg viewBox="0 0 400 260" class="h-full w-full transition duration-500 group-hover:scale-105" preserveAspectRatio="xMidYMid slice" role="img" aria-label="Contoh desain undangan seminar" xmlns="http://www.w3.org/2000/svg">
              <rect width="400" height="260" fill="#262626"/>
              <rect x="46" y="64" width="308" height="140" rx="8" fill="#fff"/>
              <path d="M46 72a8 8 0 0 1 8-8h92v140H54a8 8 0 0 1-8-8z" fill="#0A0A0A"/>
              <circle cx="96" cy="112" r="24" fill="#FF1F3D"/>
              <rect x="70" y="152" width="52" height="6" rx="3.0" fill="#fff"/>
              <rect x="76" y="166" width="40" height="4" rx="2.0" fill="#fff" opacity="0.55"/>
              <rect x="170" y="90" width="150" height="12" rx="6.0" fill="#0A0A0A"/>
              <rect x="170" y="114" width="170" height="5" rx="2.5" fill="#0A0A0A" opacity="0.35"/>
              <rect x="170" y="126" width="150" height="5" rx="2.5" fill="#0A0A0A" opacity="0.35"/>
              <rect x="170" y="138" width="160" height="5" rx="2.5" fill="#0A0A0A" opacity="0.35"/>
              <rect x="170" y="166" width="70" height="16" rx="8.0" fill="#FF1F3D"/>
            </svg>
            </button>
            <div class="p-4">
              <h3 class="text-lg font-semibold leading-snug text-white">Undangan Seminar</h3>
              <p class="mt-1 text-sm text-white/50">Undangan</p>
              <div class="mt-4 flex items-center justify-between gap-2">
                <p class="whitespace-nowrap text-[15px] font-bold text-[#ff4d5e]"><span class="block text-[11px] font-medium text-white/40">Mulai</span>Rp 90.000</p>
                <button type="button" data-add class="flex h-10 w-10 shrink-0 items-center justify-center rounded-xl border border-white/15 text-white transition hover:border-[#ff1f3d] hover:bg-[#ff1f3d]/10 hover:text-[#ff6b7a]" aria-label="Tambah Undangan Seminar ke pesanan">
                  <svg class="h-5 w-5" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" viewBox="0 0 24 24"><path d="M3 4h2l2.3 10.5a1 1 0 0 0 1 .8h8.6a1 1 0 0 0 1-.8L19 8H6.2"/><circle cx="9" cy="19.5" r="1.3"/><circle cx="17" cy="19.5" r="1.3"/></svg>
                </button>
              </div>
            </div>
          </article>

          <article class="card group overflow-hidden rounded-3xl border border-white/10 bg-[#0f0f10] transition hover:-translate-y-1 hover:border-[#ff1f3d]/40 hover:shadow-[0_0_30px_rgba(255,31,61,.15)]" data-id="b1" data-cat="banner" data-price="100000" data-title="Banner Promo Kuliner" data-desc="Lingkaran promo yang mencolok dan kontras warna tinggi agar terbaca jelas dari kejauhan." data-tags="Banner · Kuliner" data-search="banner promo kuliner banner banner · kuliner lingkaran promo yang mencolok dan kontras warna tinggi agar terbaca jelas dari kejauhan.">
            <button type="button" class="open block aspect-[4/3] w-full overflow-hidden bg-[#0c0c0d] text-left focus-visible:outline focus-visible:outline-2 focus-visible:outline-[#ff1f3d]" aria-label="Lihat detail Banner Promo Kuliner">
              <svg viewBox="0 0 400 260" class="h-full w-full transition duration-500 group-hover:scale-105" preserveAspectRatio="xMidYMid slice" role="img" aria-label="Contoh desain banner promo kuliner" xmlns="http://www.w3.org/2000/svg">
              <rect width="400" height="260" fill="#FF1F3D"/>
              <rect x="24" y="62" width="352" height="136" rx="6" fill="#0A0A0A"/>
              <circle cx="38" cy="76" r="4" fill="#FF1F3D"/><circle cx="362" cy="76" r="4" fill="#FF1F3D"/>
              <circle cx="38" cy="184" r="4" fill="#FF1F3D"/><circle cx="362" cy="184" r="4" fill="#FF1F3D"/>
              <circle cx="112" cy="130" r="40" fill="#FF1F3D"/>
              <text x="112" y="136" text-anchor="middle" font-family="Inter,Arial,sans-serif" font-size="17" font-weight="800" fill="#0A0A0A">PROMO</text>
              <rect x="170" y="100" width="170" height="14" rx="7.0" fill="#fff"/>
              <rect x="170" y="124" width="124" height="8" rx="4.0" fill="#fff" opacity="0.6"/>
              <rect x="170" y="140" width="146" height="8" rx="4.0" fill="#fff" opacity="0.6"/>
              <rect x="170" y="160" width="72" height="16" rx="8.0" fill="#FF1F3D"/>
            </svg>
            </button>
            <div class="p-4">
              <h3 class="text-lg font-semibold leading-snug text-white">Banner Promo Kuliner</h3>
              <p class="mt-1 text-sm text-white/50">Banner</p>
              <div class="mt-4 flex items-center justify-between gap-2">
                <p class="whitespace-nowrap text-[15px] font-bold text-[#ff4d5e]"><span class="block text-[11px] font-medium text-white/40">Mulai</span>Rp 100.000</p>
                <button type="button" data-add class="flex h-10 w-10 shrink-0 items-center justify-center rounded-xl border border-white/15 text-white transition hover:border-[#ff1f3d] hover:bg-[#ff1f3d]/10 hover:text-[#ff6b7a]" aria-label="Tambah Banner Promo Kuliner ke pesanan">
                  <svg class="h-5 w-5" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" viewBox="0 0 24 24"><path d="M3 4h2l2.3 10.5a1 1 0 0 0 1 .8h8.6a1 1 0 0 0 1-.8L19 8H6.2"/><circle cx="9" cy="19.5" r="1.3"/><circle cx="17" cy="19.5" r="1.3"/></svg>
                </button>
              </div>
            </div>
          </article>

          <article class="card group overflow-hidden rounded-3xl border border-white/10 bg-[#0f0f10] transition hover:-translate-y-1 hover:border-[#ff1f3d]/40 hover:shadow-[0_0_30px_rgba(255,31,61,.15)]" data-id="b2" data-cat="banner" data-price="120000" data-title="Banner Grand Opening" data-desc="Latar gelap, tulisan besar, dan bingkai putus-putus untuk menarik perhatian pada pembukaan usaha baru." data-tags="Banner · Pembukaan" data-search="banner grand opening banner banner · pembukaan latar gelap, tulisan besar, dan bingkai putus-putus untuk menarik perhatian pada pembukaan usaha baru.">
            <button type="button" class="open block aspect-[4/3] w-full overflow-hidden bg-[#0c0c0d] text-left focus-visible:outline focus-visible:outline-2 focus-visible:outline-[#ff1f3d]" aria-label="Lihat detail Banner Grand Opening">
              <svg viewBox="0 0 400 260" class="h-full w-full transition duration-500 group-hover:scale-105" preserveAspectRatio="xMidYMid slice" role="img" aria-label="Contoh desain banner grand opening" xmlns="http://www.w3.org/2000/svg">
              <rect width="400" height="260" fill="#0A0A0A"/>
              <rect x="18" y="46" width="364" height="168" rx="8" fill="none" stroke="#FF1F3D" stroke-width="3" stroke-dasharray="10 8"/>
              <circle cx="44" cy="30" r="5" fill="#FF1F3D"/><circle cx="352" cy="28" r="4" fill="#fff"/><circle cx="196" cy="24" r="4" fill="#FF1F3D"/>
              <circle cx="372" cy="236" r="5" fill="#FF1F3D"/><circle cx="36" cy="232" r="4" fill="#fff"/>
              <text x="200" y="118" text-anchor="middle" font-family="Inter,Arial,sans-serif" font-size="34" font-weight="800" fill="#fff">GRAND</text>
              <text x="200" y="154" text-anchor="middle" font-family="Inter,Arial,sans-serif" font-size="34" font-weight="800" fill="#FF1F3D">OPENING</text>
              <rect x="140" y="174" width="120" height="8" rx="4.0" fill="#fff" opacity="0.5"/>
            </svg>
            </button>
            <div class="p-4">
              <h3 class="text-lg font-semibold leading-snug text-white">Banner Grand Opening</h3>
              <p class="mt-1 text-sm text-white/50">Banner</p>
              <div class="mt-4 flex items-center justify-between gap-2">
                <p class="whitespace-nowrap text-[15px] font-bold text-[#ff4d5e]"><span class="block text-[11px] font-medium text-white/40">Mulai</span>Rp 120.000</p>
                <button type="button" data-add class="flex h-10 w-10 shrink-0 items-center justify-center rounded-xl border border-white/15 text-white transition hover:border-[#ff1f3d] hover:bg-[#ff1f3d]/10 hover:text-[#ff6b7a]" aria-label="Tambah Banner Grand Opening ke pesanan">
                  <svg class="h-5 w-5" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" viewBox="0 0 24 24"><path d="M3 4h2l2.3 10.5a1 1 0 0 0 1 .8h8.6a1 1 0 0 0 1-.8L19 8H6.2"/><circle cx="9" cy="19.5" r="1.3"/><circle cx="17" cy="19.5" r="1.3"/></svg>
                </button>
              </div>
            </div>
          </article>

          <article class="card group overflow-hidden rounded-3xl border border-white/10 bg-[#0f0f10] transition hover:-translate-y-1 hover:border-[#ff1f3d]/40 hover:shadow-[0_0_30px_rgba(255,31,61,.15)]" data-id="b3" data-cat="banner" data-price="90000" data-title="Banner Diskon" data-desc="Angka diskon besar yang langsung terlihat, cocok untuk toko, bazar, dan promo musiman." data-tags="Banner · Promosi" data-search="banner diskon banner banner · promosi angka diskon besar yang langsung terlihat, cocok untuk toko, bazar, dan promo musiman.">
            <button type="button" class="open block aspect-[4/3] w-full overflow-hidden bg-[#0c0c0d] text-left focus-visible:outline focus-visible:outline-2 focus-visible:outline-[#ff1f3d]" aria-label="Lihat detail Banner Diskon">
              <svg viewBox="0 0 400 260" class="h-full w-full transition duration-500 group-hover:scale-105" preserveAspectRatio="xMidYMid slice" role="img" aria-label="Contoh desain banner diskon" xmlns="http://www.w3.org/2000/svg">
              <rect width="400" height="260" fill="#F2F2F2"/>
              <rect x="24" y="50" width="352" height="160" rx="8" fill="#FF1F3D"/>
              <circle cx="40" cy="66" r="4" fill="#0A0A0A"/><circle cx="360" cy="66" r="4" fill="#0A0A0A"/>
              <circle cx="40" cy="194" r="4" fill="#0A0A0A"/><circle cx="360" cy="194" r="4" fill="#0A0A0A"/>
              <text x="122" y="96" text-anchor="middle" font-family="Inter,Arial,sans-serif" font-size="20" font-weight="800" fill="#0A0A0A">DISKON</text>
              <text x="122" y="164" text-anchor="middle" font-family="Inter,Arial,sans-serif" font-size="68" font-weight="900" fill="#0A0A0A">50%</text>
              <rect x="230" y="92" width="110" height="12" rx="6.0" fill="#0A0A0A"/>
              <rect x="230" y="116" width="90" height="7" rx="3.5" fill="#0A0A0A" opacity="0.55"/>
              <rect x="230" y="132" width="104" height="7" rx="3.5" fill="#0A0A0A" opacity="0.55"/>
              <rect x="230" y="158" width="84" height="18" rx="9.0" fill="#0A0A0A"/>
            </svg>
            </button>
            <div class="p-4">
              <h3 class="text-lg font-semibold leading-snug text-white">Banner Diskon</h3>
              <p class="mt-1 text-sm text-white/50">Banner</p>
              <div class="mt-4 flex items-center justify-between gap-2">
                <p class="whitespace-nowrap text-[15px] font-bold text-[#ff4d5e]"><span class="block text-[11px] font-medium text-white/40">Mulai</span>Rp 90.000</p>
                <button type="button" data-add class="flex h-10 w-10 shrink-0 items-center justify-center rounded-xl border border-white/15 text-white transition hover:border-[#ff1f3d] hover:bg-[#ff1f3d]/10 hover:text-[#ff6b7a]" aria-label="Tambah Banner Diskon ke pesanan">
                  <svg class="h-5 w-5" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" viewBox="0 0 24 24"><path d="M3 4h2l2.3 10.5a1 1 0 0 0 1 .8h8.6a1 1 0 0 0 1-.8L19 8H6.2"/><circle cx="9" cy="19.5" r="1.3"/><circle cx="17" cy="19.5" r="1.3"/></svg>
                </button>
              </div>
            </div>
          </article>

          <article class="card group overflow-hidden rounded-3xl border border-white/10 bg-[#0f0f10] transition hover:-translate-y-1 hover:border-[#ff1f3d]/40 hover:shadow-[0_0_30px_rgba(255,31,61,.15)]" data-id="b4" data-cat="banner" data-price="130000" data-title="Spanduk Acara" data-desc="Spanduk memanjang dengan garis penegas dan area logo untuk kegiatan, lomba, dan acara komunitas." data-tags="Banner · Spanduk" data-search="spanduk acara banner banner · spanduk spanduk memanjang dengan garis penegas dan area logo untuk kegiatan, lomba, dan acara komunitas.">
            <button type="button" class="open block aspect-[4/3] w-full overflow-hidden bg-[#0c0c0d] text-left focus-visible:outline focus-visible:outline-2 focus-visible:outline-[#ff1f3d]" aria-label="Lihat detail Spanduk Acara">
              <svg viewBox="0 0 400 260" class="h-full w-full transition duration-500 group-hover:scale-105" preserveAspectRatio="xMidYMid slice" role="img" aria-label="Contoh desain spanduk acara" xmlns="http://www.w3.org/2000/svg">
              <rect width="400" height="260" fill="#F2F2F2"/>
              <rect x="18" y="40" width="8" height="210" rx="2" fill="#A3A3A3"/>
              <rect x="374" y="40" width="8" height="210" rx="2" fill="#A3A3A3"/>
              <rect x="26" y="84" width="348" height="96" fill="#0A0A0A"/>
              <rect x="26" y="84" width="348" height="8" fill="#FF1F3D"/>
              <rect x="26" y="172" width="348" height="8" fill="#FF1F3D"/>
              <circle cx="76" cy="132" r="24" fill="#FF1F3D"/>
              <rect x="118" y="112" width="200" height="14" rx="7.0" fill="#fff"/>
              <rect x="118" y="136" width="150" height="8" rx="4.0" fill="#fff" opacity="0.6"/>
              <rect x="118" y="152" width="170" height="8" rx="4.0" fill="#fff" opacity="0.6"/>
            </svg>
            </button>
            <div class="p-4">
              <h3 class="text-lg font-semibold leading-snug text-white">Spanduk Acara</h3>
              <p class="mt-1 text-sm text-white/50">Banner</p>
              <div class="mt-4 flex items-center justify-between gap-2">
                <p class="whitespace-nowrap text-[15px] font-bold text-[#ff4d5e]"><span class="block text-[11px] font-medium text-white/40">Mulai</span>Rp 130.000</p>
                <button type="button" data-add class="flex h-10 w-10 shrink-0 items-center justify-center rounded-xl border border-white/15 text-white transition hover:border-[#ff1f3d] hover:bg-[#ff1f3d]/10 hover:text-[#ff6b7a]" aria-label="Tambah Spanduk Acara ke pesanan">
                  <svg class="h-5 w-5" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" viewBox="0 0 24 24"><path d="M3 4h2l2.3 10.5a1 1 0 0 0 1 .8h8.6a1 1 0 0 0 1-.8L19 8H6.2"/><circle cx="9" cy="19.5" r="1.3"/><circle cx="17" cy="19.5" r="1.3"/></svg>
                </button>
              </div>
            </div>
          </article>

          <article class="card group overflow-hidden rounded-3xl border border-white/10 bg-[#0f0f10] transition hover:-translate-y-1 hover:border-[#ff1f3d]/40 hover:shadow-[0_0_30px_rgba(255,31,61,.15)]" data-id="l1" data-cat="logo" data-price="150000" data-title="Logo Geometris" data-desc="Perpaduan lingkaran dan bentuk berlian yang simpel, tegas, dan mudah dikenali di berbagai ukuran." data-tags="Logo · Ikon" data-search="logo geometris logo logo · ikon perpaduan lingkaran dan bentuk berlian yang simpel, tegas, dan mudah dikenali di berbagai ukuran.">
            <button type="button" class="open block aspect-[4/3] w-full overflow-hidden bg-[#0c0c0d] text-left focus-visible:outline focus-visible:outline-2 focus-visible:outline-[#ff1f3d]" aria-label="Lihat detail Logo Geometris">
              <svg viewBox="0 0 400 260" class="h-full w-full transition duration-500 group-hover:scale-105" preserveAspectRatio="xMidYMid slice" role="img" aria-label="Contoh desain logo geometris" xmlns="http://www.w3.org/2000/svg">
              <rect width="400" height="260" fill="#F2F2F2"/>
              <rect x="28" y="28" width="52" height="52" rx="10" fill="#0A0A0A"/><circle cx="54" cy="54" r="12" fill="#FF1F3D"/>
              <rect x="320" y="28" width="52" height="52" rx="10" fill="#FF1F3D"/><circle cx="346" cy="54" r="12" fill="#0A0A0A"/>
              <circle cx="200" cy="108" r="46" fill="#0A0A0A"/>
              <rect x="176" y="84" width="48" height="48" rx="8" fill="#FF1F3D" transform="rotate(45 200 108)"/>
              <circle cx="200" cy="108" r="14" fill="#0A0A0A"/>
              <rect x="150" y="178" width="100" height="10" rx="5.0" fill="#0A0A0A"/>
              <rect x="170" y="196" width="60" height="6" rx="3.0" fill="#0A0A0A" opacity="0.4"/>
            </svg>
            </button>
            <div class="p-4">
              <h3 class="text-lg font-semibold leading-snug text-white">Logo Geometris</h3>
              <p class="mt-1 text-sm text-white/50">Logo</p>
              <div class="mt-4 flex items-center justify-between gap-2">
                <p class="whitespace-nowrap text-[15px] font-bold text-[#ff4d5e]"><span class="block text-[11px] font-medium text-white/40">Mulai</span>Rp 150.000</p>
                <button type="button" data-add class="flex h-10 w-10 shrink-0 items-center justify-center rounded-xl border border-white/15 text-white transition hover:border-[#ff1f3d] hover:bg-[#ff1f3d]/10 hover:text-[#ff6b7a]" aria-label="Tambah Logo Geometris ke pesanan">
                  <svg class="h-5 w-5" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" viewBox="0 0 24 24"><path d="M3 4h2l2.3 10.5a1 1 0 0 0 1 .8h8.6a1 1 0 0 0 1-.8L19 8H6.2"/><circle cx="9" cy="19.5" r="1.3"/><circle cx="17" cy="19.5" r="1.3"/></svg>
                </button>
              </div>
            </div>
          </article>

          <article class="card group overflow-hidden rounded-3xl border border-white/10 bg-[#0f0f10] transition hover:-translate-y-1 hover:border-[#ff1f3d]/40 hover:shadow-[0_0_30px_rgba(255,31,61,.15)]" data-id="l2" data-cat="logo" data-price="175000" data-title="Logo Kuliner" data-desc="Ikon mangkuk dengan uap hangat dalam lencana bulat untuk warung, kafe, dan usaha makanan." data-tags="Logo · Kuliner" data-search="logo kuliner logo logo · kuliner ikon mangkuk dengan uap hangat dalam lencana bulat untuk warung, kafe, dan usaha makanan.">
            <button type="button" class="open block aspect-[4/3] w-full overflow-hidden bg-[#0c0c0d] text-left focus-visible:outline focus-visible:outline-2 focus-visible:outline-[#ff1f3d]" aria-label="Lihat detail Logo Kuliner">
              <svg viewBox="0 0 400 260" class="h-full w-full transition duration-500 group-hover:scale-105" preserveAspectRatio="xMidYMid slice" role="img" aria-label="Contoh desain logo kuliner" xmlns="http://www.w3.org/2000/svg">
              <rect width="400" height="260" fill="#F2F2F2"/>
              <circle cx="200" cy="108" r="62" fill="#0A0A0A"/>
              <path d="M156 112h88a44 44 0 0 1-88 0z" fill="#FF1F3D"/>
              <path d="M178 98q-9-12 0-24M200 98q-9-12 0-24M222 98q-9-12 0-24" stroke="#fff" stroke-width="4" fill="none" stroke-linecap="round"/>
              <rect x="164" y="192" width="72" height="10" rx="5.0" fill="#0A0A0A"/>
              <rect x="180" y="210" width="40" height="6" rx="3.0" fill="#0A0A0A" opacity="0.4"/>
            </svg>
            </button>
            <div class="p-4">
              <h3 class="text-lg font-semibold leading-snug text-white">Logo Kuliner</h3>
              <p class="mt-1 text-sm text-white/50">Logo</p>
              <div class="mt-4 flex items-center justify-between gap-2">
                <p class="whitespace-nowrap text-[15px] font-bold text-[#ff4d5e]"><span class="block text-[11px] font-medium text-white/40">Mulai</span>Rp 175.000</p>
                <button type="button" data-add class="flex h-10 w-10 shrink-0 items-center justify-center rounded-xl border border-white/15 text-white transition hover:border-[#ff1f3d] hover:bg-[#ff1f3d]/10 hover:text-[#ff6b7a]" aria-label="Tambah Logo Kuliner ke pesanan">
                  <svg class="h-5 w-5" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" viewBox="0 0 24 24"><path d="M3 4h2l2.3 10.5a1 1 0 0 0 1 .8h8.6a1 1 0 0 0 1-.8L19 8H6.2"/><circle cx="9" cy="19.5" r="1.3"/><circle cx="17" cy="19.5" r="1.3"/></svg>
                </button>
              </div>
            </div>
          </article>

          <article class="card group overflow-hidden rounded-3xl border border-white/10 bg-[#0f0f10] transition hover:-translate-y-1 hover:border-[#ff1f3d]/40 hover:shadow-[0_0_30px_rgba(255,31,61,.15)]" data-id="l3" data-cat="logo" data-price="200000" data-title="Logo Emblem" data-desc="Lambang bulat berbingkai dengan bintang di tengah yang memberi kesan resmi dan terpercaya." data-tags="Logo · Emblem" data-search="logo emblem logo logo · emblem lambang bulat berbingkai dengan bintang di tengah yang memberi kesan resmi dan terpercaya.">
            <button type="button" class="open block aspect-[4/3] w-full overflow-hidden bg-[#0c0c0d] text-left focus-visible:outline focus-visible:outline-2 focus-visible:outline-[#ff1f3d]" aria-label="Lihat detail Logo Emblem">
              <svg viewBox="0 0 400 260" class="h-full w-full transition duration-500 group-hover:scale-105" preserveAspectRatio="xMidYMid slice" role="img" aria-label="Contoh desain logo emblem" xmlns="http://www.w3.org/2000/svg">
              <rect width="400" height="260" fill="#F2F2F2"/>
              <circle cx="200" cy="108" r="70" fill="none" stroke="#0A0A0A" stroke-width="6"/>
              <circle cx="200" cy="108" r="56" fill="#0A0A0A"/>
              <circle cx="200" cy="108" r="46" fill="none" stroke="#FF1F3D" stroke-width="1.5" stroke-dasharray="3 5"/>
              <polygon points="200.0,80.0 207.1,98.3 226.6,99.3 211.4,111.7 216.5,130.7 200.0,120.0 183.5,130.7 188.6,111.7 173.4,99.3 192.9,98.3" fill="#FF1F3D"/>
              <rect x="160" y="194" width="80" height="10" rx="5.0" fill="#0A0A0A"/>
              <rect x="176" y="212" width="48" height="6" rx="3.0" fill="#0A0A0A" opacity="0.4"/>
            </svg>
            </button>
            <div class="p-4">
              <h3 class="text-lg font-semibold leading-snug text-white">Logo Emblem</h3>
              <p class="mt-1 text-sm text-white/50">Logo</p>
              <div class="mt-4 flex items-center justify-between gap-2">
                <p class="whitespace-nowrap text-[15px] font-bold text-[#ff4d5e]"><span class="block text-[11px] font-medium text-white/40">Mulai</span>Rp 200.000</p>
                <button type="button" data-add class="flex h-10 w-10 shrink-0 items-center justify-center rounded-xl border border-white/15 text-white transition hover:border-[#ff1f3d] hover:bg-[#ff1f3d]/10 hover:text-[#ff6b7a]" aria-label="Tambah Logo Emblem ke pesanan">
                  <svg class="h-5 w-5" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" viewBox="0 0 24 24"><path d="M3 4h2l2.3 10.5a1 1 0 0 0 1 .8h8.6a1 1 0 0 0 1-.8L19 8H6.2"/><circle cx="9" cy="19.5" r="1.3"/><circle cx="17" cy="19.5" r="1.3"/></svg>
                </button>
              </div>
            </div>
          </article>

          <article class="card group overflow-hidden rounded-3xl border border-white/10 bg-[#0f0f10] transition hover:-translate-y-1 hover:border-[#ff1f3d]/40 hover:shadow-[0_0_30px_rgba(255,31,61,.15)]" data-id="l4" data-cat="logo" data-price="125000" data-title="Logo Wordmark" data-desc="Logo berbasis tulisan dengan ikon pendamping, lengkap dengan versi latar terang dan gelap." data-tags="Logo · Wordmark" data-search="logo wordmark logo logo · wordmark logo berbasis tulisan dengan ikon pendamping, lengkap dengan versi latar terang dan gelap.">
            <button type="button" class="open block aspect-[4/3] w-full overflow-hidden bg-[#0c0c0d] text-left focus-visible:outline focus-visible:outline-2 focus-visible:outline-[#ff1f3d]" aria-label="Lihat detail Logo Wordmark">
              <svg viewBox="0 0 400 260" class="h-full w-full transition duration-500 group-hover:scale-105" preserveAspectRatio="xMidYMid slice" role="img" aria-label="Contoh desain logo wordmark" xmlns="http://www.w3.org/2000/svg">
              <rect width="400" height="260" fill="#F2F2F2"/>
              <rect x="84" y="50" width="56" height="56" rx="14" fill="#0A0A0A"/>
              <circle cx="112" cy="78" r="13" fill="#FF1F3D"/>
              <rect x="156" y="58" width="150" height="18" rx="9.0" fill="#0A0A0A"/>
              <circle cx="316" cy="67" r="6" fill="#FF1F3D"/>
              <rect x="156" y="86" width="100" height="8" rx="4.0" fill="#0A0A0A" opacity="0.4"/>
              <rect x="60" y="150" width="280" height="76" rx="12" fill="#0A0A0A"/>
              <rect x="92" y="172" width="32" height="32" rx="9" fill="#FF1F3D"/>
              <circle cx="108" cy="188" r="8" fill="#0A0A0A"/>
              <rect x="138" y="174" width="110" height="12" rx="6.0" fill="#fff"/>
              <rect x="138" y="194" width="70" height="6" rx="3.0" fill="#fff" opacity="0.55"/>
            </svg>
            </button>
            <div class="p-4">
              <h3 class="text-lg font-semibold leading-snug text-white">Logo Wordmark</h3>
              <p class="mt-1 text-sm text-white/50">Logo</p>
              <div class="mt-4 flex items-center justify-between gap-2">
                <p class="whitespace-nowrap text-[15px] font-bold text-[#ff4d5e]"><span class="block text-[11px] font-medium text-white/40">Mulai</span>Rp 125.000</p>
                <button type="button" data-add class="flex h-10 w-10 shrink-0 items-center justify-center rounded-xl border border-white/15 text-white transition hover:border-[#ff1f3d] hover:bg-[#ff1f3d]/10 hover:text-[#ff6b7a]" aria-label="Tambah Logo Wordmark ke pesanan">
                  <svg class="h-5 w-5" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" viewBox="0 0 24 24"><path d="M3 4h2l2.3 10.5a1 1 0 0 0 1 .8h8.6a1 1 0 0 0 1-.8L19 8H6.2"/><circle cx="9" cy="19.5" r="1.3"/><circle cx="17" cy="19.5" r="1.3"/></svg>
                </button>
              </div>
            </div>
          </article>

          <article class="card group overflow-hidden rounded-3xl border border-white/10 bg-[#0f0f10] transition hover:-translate-y-1 hover:border-[#ff1f3d]/40 hover:shadow-[0_0_30px_rgba(255,31,61,.15)]" data-id="c1" data-cat="compro" data-price="450000" data-title="Compro Perusahaan" data-desc="Halaman terbuka yang menampilkan profil usaha, foto utama, dan teks yang tertata rapi." data-tags="Compro · Profil Usaha" data-search="compro perusahaan company profile compro · profil usaha halaman terbuka yang menampilkan profil usaha, foto utama, dan teks yang tertata rapi.">
            <button type="button" class="open block aspect-[4/3] w-full overflow-hidden bg-[#0c0c0d] text-left focus-visible:outline focus-visible:outline-2 focus-visible:outline-[#ff1f3d]" aria-label="Lihat detail Compro Perusahaan">
              <svg viewBox="0 0 400 260" class="h-full w-full transition duration-500 group-hover:scale-105" preserveAspectRatio="xMidYMid slice" role="img" aria-label="Contoh desain company profile" xmlns="http://www.w3.org/2000/svg">
              <rect width="400" height="260" fill="#262626"/>
              <rect x="52" y="34" width="148" height="192" rx="4" fill="#fff"/>
              <rect x="200" y="34" width="148" height="192" rx="4" fill="#F5F5F5"/>
              <rect x="199" y="34" width="2" height="192" fill="#0A0A0A" opacity=".15"/>
              <rect x="66" y="48" width="120" height="58" rx="3" fill="#FF1F3D"/>
              <rect x="66" y="48" width="44" height="58" rx="3" fill="#0A0A0A"/>
              <rect x="66" y="120" width="90" height="9" rx="4.5" fill="#0A0A0A"/>
              <rect x="66" y="138" width="116" height="5" rx="2.5" fill="#0A0A0A" opacity="0.3"/>
              <rect x="66" y="150" width="104" height="5" rx="2.5" fill="#0A0A0A" opacity="0.3"/>
              <rect x="66" y="162" width="112" height="5" rx="2.5" fill="#0A0A0A" opacity="0.3"/>
              <rect x="216" y="50" width="54" height="40" rx="3" fill="#0A0A0A"/>
              <rect x="278" y="50" width="54" height="40" rx="3" fill="#FF1F3D"/>
              <rect x="216" y="98" width="54" height="40" rx="3" fill="#FF1F3D"/>
              <rect x="278" y="98" width="54" height="40" rx="3" fill="#0A0A0A"/>
              <rect x="216" y="154" width="112" height="6" rx="3.0" fill="#0A0A0A" opacity="0.35"/>
              <rect x="216" y="168" width="96" height="6" rx="3.0" fill="#0A0A0A" opacity="0.35"/>
              <rect x="216" y="182" width="104" height="6" rx="3.0" fill="#0A0A0A" opacity="0.35"/>
            </svg>
            </button>
            <div class="p-4">
              <h3 class="text-lg font-semibold leading-snug text-white">Compro Perusahaan</h3>
              <p class="mt-1 text-sm text-white/50">Company Profile</p>
              <div class="mt-4 flex items-center justify-between gap-2">
                <p class="whitespace-nowrap text-[15px] font-bold text-[#ff4d5e]"><span class="block text-[11px] font-medium text-white/40">Mulai</span>Rp 450.000</p>
                <button type="button" data-add class="flex h-10 w-10 shrink-0 items-center justify-center rounded-xl border border-white/15 text-white transition hover:border-[#ff1f3d] hover:bg-[#ff1f3d]/10 hover:text-[#ff6b7a]" aria-label="Tambah Compro Perusahaan ke pesanan">
                  <svg class="h-5 w-5" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" viewBox="0 0 24 24"><path d="M3 4h2l2.3 10.5a1 1 0 0 0 1 .8h8.6a1 1 0 0 0 1-.8L19 8H6.2"/><circle cx="9" cy="19.5" r="1.3"/><circle cx="17" cy="19.5" r="1.3"/></svg>
                </button>
              </div>
            </div>
          </article>

          <article class="card group overflow-hidden rounded-3xl border border-white/10 bg-[#0f0f10] transition hover:-translate-y-1 hover:border-[#ff1f3d]/40 hover:shadow-[0_0_30px_rgba(255,31,61,.15)]" data-id="c2" data-cat="compro" data-price="250000" data-title="Cover Compro" data-desc="Sampul bersih dengan bidang warna diagonal yang memberi kesan modern dan profesional." data-tags="Compro · Sampul" data-search="cover compro company profile compro · sampul sampul bersih dengan bidang warna diagonal yang memberi kesan modern dan profesional.">
            <button type="button" class="open block aspect-[4/3] w-full overflow-hidden bg-[#0c0c0d] text-left focus-visible:outline focus-visible:outline-2 focus-visible:outline-[#ff1f3d]" aria-label="Lihat detail Cover Compro">
              <svg viewBox="0 0 400 260" class="h-full w-full transition duration-500 group-hover:scale-105" preserveAspectRatio="xMidYMid slice" role="img" aria-label="Contoh desain cover company profile" xmlns="http://www.w3.org/2000/svg">
              <rect width="400" height="260" fill="#F2F2F2"/>
              <rect x="150" y="30" width="140" height="214" rx="5" fill="#D4D4D4"/>
              <rect x="124" y="20" width="140" height="214" rx="5" fill="#0A0A0A"/>
              <polygon points="124,160 264,108 264,234 124,234" fill="#FF1F3D"/>
              <circle cx="160" cy="62" r="16" fill="none" stroke="#FF1F3D" stroke-width="3"/>
              <circle cx="160" cy="62" r="5" fill="#FF1F3D"/>
              <rect x="146" y="100" width="86" height="10" rx="5.0" fill="#fff"/>
              <rect x="146" y="118" width="60" height="6" rx="3.0" fill="#fff" opacity="0.55"/>
              <rect x="150" y="196" width="70" height="8" rx="4.0" fill="#0A0A0A"/>
            </svg>
            </button>
            <div class="p-4">
              <h3 class="text-lg font-semibold leading-snug text-white">Cover Compro</h3>
              <p class="mt-1 text-sm text-white/50">Company Profile</p>
              <div class="mt-4 flex items-center justify-between gap-2">
                <p class="whitespace-nowrap text-[15px] font-bold text-[#ff4d5e]"><span class="block text-[11px] font-medium text-white/40">Mulai</span>Rp 250.000</p>
                <button type="button" data-add class="flex h-10 w-10 shrink-0 items-center justify-center rounded-xl border border-white/15 text-white transition hover:border-[#ff1f3d] hover:bg-[#ff1f3d]/10 hover:text-[#ff6b7a]" aria-label="Tambah Cover Compro ke pesanan">
                  <svg class="h-5 w-5" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" viewBox="0 0 24 24"><path d="M3 4h2l2.3 10.5a1 1 0 0 0 1 .8h8.6a1 1 0 0 0 1-.8L19 8H6.2"/><circle cx="9" cy="19.5" r="1.3"/><circle cx="17" cy="19.5" r="1.3"/></svg>
                </button>
              </div>
            </div>
          </article>

          <article class="card group overflow-hidden rounded-3xl border border-white/10 bg-[#0f0f10] transition hover:-translate-y-1 hover:border-[#ff1f3d]/40 hover:shadow-[0_0_30px_rgba(255,31,61,.15)]" data-id="c3" data-cat="compro" data-price="300000" data-title="Halaman Layanan" data-desc="Daftar layanan dengan ikon dan penjelasan singkat dalam tiga kolom yang seimbang." data-tags="Compro · Layanan" data-search="halaman layanan company profile compro · layanan daftar layanan dengan ikon dan penjelasan singkat dalam tiga kolom yang seimbang.">
            <button type="button" class="open block aspect-[4/3] w-full overflow-hidden bg-[#0c0c0d] text-left focus-visible:outline focus-visible:outline-2 focus-visible:outline-[#ff1f3d]" aria-label="Lihat detail Halaman Layanan">
              <svg viewBox="0 0 400 260" class="h-full w-full transition duration-500 group-hover:scale-105" preserveAspectRatio="xMidYMid slice" role="img" aria-label="Contoh desain halaman layanan company profile" xmlns="http://www.w3.org/2000/svg">
              <rect width="400" height="260" fill="#262626"/>
              <rect x="56" y="28" width="288" height="204" rx="6" fill="#fff"/>
              <rect x="56" y="28" width="288" height="36" rx="6" fill="#FF1F3D"/>
              <rect x="74" y="42" width="100" height="8" rx="4.0" fill="#0A0A0A"/>
              <circle cx="102" cy="108" r="17" fill="#0A0A0A"/><circle cx="102" cy="108" r="6" fill="#FF1F3D"/>
              <circle cx="200" cy="108" r="17" fill="#0A0A0A"/><circle cx="200" cy="108" r="6" fill="#FF1F3D"/>
              <circle cx="298" cy="108" r="17" fill="#0A0A0A"/><circle cx="298" cy="108" r="6" fill="#FF1F3D"/>
              <rect x="78" y="140" width="48" height="7" rx="3.5" fill="#0A0A0A"/><rect x="176" y="140" width="48" height="7" rx="3.5" fill="#0A0A0A"/><rect x="274" y="140" width="48" height="7" rx="3.5" fill="#0A0A0A"/>
              <rect x="74" y="156" width="56" height="4" rx="2.0" fill="#0A0A0A" opacity="0.3"/><rect x="172" y="156" width="56" height="4" rx="2.0" fill="#0A0A0A" opacity="0.3"/><rect x="270" y="156" width="56" height="4" rx="2.0" fill="#0A0A0A" opacity="0.3"/>
              <rect x="78" y="168" width="48" height="4" rx="2.0" fill="#0A0A0A" opacity="0.3"/><rect x="176" y="168" width="48" height="4" rx="2.0" fill="#0A0A0A" opacity="0.3"/><rect x="274" y="168" width="48" height="4" rx="2.0" fill="#0A0A0A" opacity="0.3"/>
              <rect x="74" y="198" width="70" height="12" rx="6.0" fill="#FF1F3D"/>
            </svg>
            </button>
            <div class="p-4">
              <h3 class="text-lg font-semibold leading-snug text-white">Halaman Layanan</h3>
              <p class="mt-1 text-sm text-white/50">Company Profile</p>
              <div class="mt-4 flex items-center justify-between gap-2">
                <p class="whitespace-nowrap text-[15px] font-bold text-[#ff4d5e]"><span class="block text-[11px] font-medium text-white/40">Mulai</span>Rp 300.000</p>
                <button type="button" data-add class="flex h-10 w-10 shrink-0 items-center justify-center rounded-xl border border-white/15 text-white transition hover:border-[#ff1f3d] hover:bg-[#ff1f3d]/10 hover:text-[#ff6b7a]" aria-label="Tambah Halaman Layanan ke pesanan">
                  <svg class="h-5 w-5" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" viewBox="0 0 24 24"><path d="M3 4h2l2.3 10.5a1 1 0 0 0 1 .8h8.6a1 1 0 0 0 1-.8L19 8H6.2"/><circle cx="9" cy="19.5" r="1.3"/><circle cx="17" cy="19.5" r="1.3"/></svg>
                </button>
              </div>
            </div>
          </article>

          <article class="card group overflow-hidden rounded-3xl border border-white/10 bg-[#0f0f10] transition hover:-translate-y-1 hover:border-[#ff1f3d]/40 hover:shadow-[0_0_30px_rgba(255,31,61,.15)]" data-id="c4" data-cat="compro" data-price="350000" data-title="Katalog Produk" data-desc="Tata letak katalog dengan foto produk dan harga yang mudah dipindai pelanggan." data-tags="Compro · Katalog" data-search="katalog produk company profile compro · katalog tata letak katalog dengan foto produk dan harga yang mudah dipindai pelanggan.">
            <button type="button" class="open block aspect-[4/3] w-full overflow-hidden bg-[#0c0c0d] text-left focus-visible:outline focus-visible:outline-2 focus-visible:outline-[#ff1f3d]" aria-label="Lihat detail Katalog Produk">
              <svg viewBox="0 0 400 260" class="h-full w-full transition duration-500 group-hover:scale-105" preserveAspectRatio="xMidYMid slice" role="img" aria-label="Contoh desain katalog produk" xmlns="http://www.w3.org/2000/svg">
              <rect width="400" height="260" fill="#F2F2F2"/>
              <rect x="52" y="20" width="296" height="224" rx="6" fill="#fff"/>
              <rect x="72" y="32" width="90" height="8" rx="4.0" fill="#0A0A0A"/>
              <rect x="72" y="60" width="76" height="56" rx="4" fill="#0A0A0A"/>
              <rect x="72" y="124" width="50" height="7" rx="3.5" fill="#0A0A0A" opacity="0.45"/>
              <rect x="72" y="136" width="30" height="6" rx="3.0" fill="#FF1F3D"/>
              <rect x="162" y="60" width="76" height="56" rx="4" fill="#FF1F3D"/>
              <rect x="162" y="124" width="50" height="7" rx="3.5" fill="#0A0A0A" opacity="0.45"/>
              <rect x="162" y="136" width="30" height="6" rx="3.0" fill="#FF1F3D"/>
              <rect x="252" y="60" width="76" height="56" rx="4" fill="#0A0A0A"/>
              <rect x="252" y="124" width="50" height="7" rx="3.5" fill="#0A0A0A" opacity="0.45"/>
              <rect x="252" y="136" width="30" height="6" rx="3.0" fill="#FF1F3D"/>
              <rect x="72" y="146" width="76" height="56" rx="4" fill="#FF1F3D"/>
              <rect x="72" y="210" width="50" height="7" rx="3.5" fill="#0A0A0A" opacity="0.45"/>
              <rect x="72" y="222" width="30" height="6" rx="3.0" fill="#FF1F3D"/>
              <rect x="162" y="146" width="76" height="56" rx="4" fill="#0A0A0A"/>
              <rect x="162" y="210" width="50" height="7" rx="3.5" fill="#0A0A0A" opacity="0.45"/>
              <rect x="162" y="222" width="30" height="6" rx="3.0" fill="#FF1F3D"/>
              <rect x="252" y="146" width="76" height="56" rx="4" fill="#FF1F3D"/>
              <rect x="252" y="210" width="50" height="7" rx="3.5" fill="#0A0A0A" opacity="0.45"/>
              <rect x="252" y="222" width="30" height="6" rx="3.0" fill="#FF1F3D"/>
            </svg>
            </button>
            <div class="p-4">
              <h3 class="text-lg font-semibold leading-snug text-white">Katalog Produk</h3>
              <p class="mt-1 text-sm text-white/50">Company Profile</p>
              <div class="mt-4 flex items-center justify-between gap-2">
                <p class="whitespace-nowrap text-[15px] font-bold text-[#ff4d5e]"><span class="block text-[11px] font-medium text-white/40">Mulai</span>Rp 350.000</p>
                <button type="button" data-add class="flex h-10 w-10 shrink-0 items-center justify-center rounded-xl border border-white/15 text-white transition hover:border-[#ff1f3d] hover:bg-[#ff1f3d]/10 hover:text-[#ff6b7a]" aria-label="Tambah Katalog Produk ke pesanan">
                  <svg class="h-5 w-5" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" viewBox="0 0 24 24"><path d="M3 4h2l2.3 10.5a1 1 0 0 0 1 .8h8.6a1 1 0 0 0 1-.8L19 8H6.2"/><circle cx="9" cy="19.5" r="1.3"/><circle cx="17" cy="19.5" r="1.3"/></svg>
                </button>
              </div>
            </div>
          </article>
      </div>
      <p id="emptyMsg" class="mt-10 hidden rounded-2xl border border-white/10 bg-white/5 p-8 text-center text-white/60">Tidak ada desain yang cocok. Coba kata kunci lain.</p>
    </section>

    <!-- GALERI -->
    <section id="galeri" class="mx-auto max-w-6xl px-5 pt-24">
      <div class="reveal mb-8">
        <p class="text-sm font-semibold uppercase tracking-[.25em] text-[#ff6b7a]">Galeri</p>
        <h2 class="mt-3 text-4xl font-semibold text-white sm:text-5xl">Sampel Terbaru</h2>
        <p class="mt-3 max-w-xl text-white/60">Ketuk salah satunya untuk melihat kategorinya di katalog.</p>
      </div>
      <div class="grid grid-cols-2 gap-3 sm:grid-cols-3 sm:gap-4 lg:grid-cols-5">
        <a href="#katalog" data-gcat="undangan" class="gal reveal group relative block overflow-hidden rounded-2xl border border-white/10 transition hover:-translate-y-1 hover:border-[#ff1f3d]/40 focus-visible:outline focus-visible:outline-2 focus-visible:outline-[#ff1f3d]" aria-label="Undangan Pernikahan, buka katalog Undangan">
          <div class="aspect-[3/4] overflow-hidden bg-[#0c0c0d]">
            <svg viewBox="0 0 300 400" class="h-full w-full transition duration-500 group-hover:scale-105" preserveAspectRatio="xMidYMid slice" role="img" aria-label="Undangan pernikahan" xmlns="http://www.w3.org/2000/svg">
            <rect width="300" height="400" fill="#0A0A0A"/>
            <rect x="40" y="40" width="220" height="320" rx="8" fill="#FFF5F5"/>
            <rect x="52" y="52" width="196" height="296" rx="4" fill="none" stroke="#FF1F3D" stroke-width="2"/>
            <circle cx="150" cy="130" r="32" fill="none" stroke="#FF1F3D" stroke-width="3"/><circle cx="150" cy="130" r="12" fill="#FF1F3D"/>
            <rect x="100" y="196" width="100" height="10" rx="5.0" fill="#0A0A0A"/><rect x="80" y="220" width="140" height="6" rx="3.0" fill="#0A0A0A" opacity="0.35"/><rect x="92" y="236" width="116" height="6" rx="3.0" fill="#0A0A0A" opacity="0.35"/><rect x="108" y="296" width="84" height="18" rx="9.0" fill="#FF1F3D"/>
          </svg>
          </div>
          <div class="pointer-events-none absolute inset-x-0 bottom-0 bg-gradient-to-t from-[#050505] to-transparent px-3 pb-3 pt-12">
            <p class="text-[10px] font-semibold uppercase tracking-wider text-[#ff6b7a]">Undangan</p>
            <p class="text-base font-bold leading-tight text-white">Undangan Pernikahan</p>
          </div>
        </a>

        <a href="#katalog" data-gcat="banner" class="gal reveal group relative block overflow-hidden rounded-2xl border border-white/10 transition hover:-translate-y-1 hover:border-[#ff1f3d]/40 focus-visible:outline focus-visible:outline-2 focus-visible:outline-[#ff1f3d]" aria-label="Roll Banner Promo, buka katalog Banner">
          <div class="aspect-[3/4] overflow-hidden bg-[#0c0c0d]">
            <svg viewBox="0 0 300 400" class="h-full w-full transition duration-500 group-hover:scale-105" preserveAspectRatio="xMidYMid slice" role="img" aria-label="Roll banner promo" xmlns="http://www.w3.org/2000/svg">
            <rect width="300" height="400" fill="#F2F2F2"/>
            <rect x="70" y="24" width="160" height="330" fill="#0A0A0A"/>
            <rect x="70" y="24" width="160" height="12" fill="#FF1F3D"/>
            <circle cx="150" cy="120" r="38" fill="#FF1F3D"/>
            <text x="150" y="127" text-anchor="middle" font-family="Inter,Arial,sans-serif" font-size="20" font-weight="800" fill="#0A0A0A">PROMO</text>
            <rect x="96" y="190" width="108" height="12" rx="6.0" fill="#fff"/><rect x="96" y="214" width="84" height="7" rx="3.5" fill="#fff" opacity="0.55"/><rect x="96" y="230" width="96" height="7" rx="3.5" fill="#fff" opacity="0.55"/><rect x="106" y="290" width="88" height="18" rx="9.0" fill="#FF1F3D"/>
            <rect x="60" y="354" width="180" height="14" rx="3" fill="#A3A3A3"/>
          </svg>
          </div>
          <div class="pointer-events-none absolute inset-x-0 bottom-0 bg-gradient-to-t from-[#050505] to-transparent px-3 pb-3 pt-12">
            <p class="text-[10px] font-semibold uppercase tracking-wider text-[#ff6b7a]">Banner</p>
            <p class="text-base font-bold leading-tight text-white">Roll Banner Promo</p>
          </div>
        </a>

        <a href="#katalog" data-gcat="logo" class="gal reveal group relative block overflow-hidden rounded-2xl border border-white/10 transition hover:-translate-y-1 hover:border-[#ff1f3d]/40 focus-visible:outline focus-visible:outline-2 focus-visible:outline-[#ff1f3d]" aria-label="Logo Geometris, buka katalog Logo">
          <div class="aspect-[3/4] overflow-hidden bg-[#0c0c0d]">
            <svg viewBox="0 0 300 400" class="h-full w-full transition duration-500 group-hover:scale-105" preserveAspectRatio="xMidYMid slice" role="img" aria-label="Logo geometris" xmlns="http://www.w3.org/2000/svg">
            <rect width="300" height="400" fill="#F2F2F2"/>
            <circle cx="150" cy="170" r="70" fill="#0A0A0A"/>
            <rect x="114" y="134" width="72" height="72" rx="10" fill="#FF1F3D" transform="rotate(45 150 170)"/>
            <circle cx="150" cy="170" r="20" fill="#0A0A0A"/>
            <rect x="100" y="274" width="100" height="12" rx="6.0" fill="#0A0A0A"/><rect x="122" y="298" width="56" height="7" rx="3.5" fill="#0A0A0A" opacity="0.4"/>
          </svg>
          </div>
          <div class="pointer-events-none absolute inset-x-0 bottom-0 bg-gradient-to-t from-[#050505] to-transparent px-3 pb-3 pt-12">
            <p class="text-[10px] font-semibold uppercase tracking-wider text-[#ff6b7a]">Logo</p>
            <p class="text-base font-bold leading-tight text-white">Logo Geometris</p>
          </div>
        </a>

        <a href="#katalog" data-gcat="compro" class="gal reveal group relative block overflow-hidden rounded-2xl border border-white/10 transition hover:-translate-y-1 hover:border-[#ff1f3d]/40 focus-visible:outline focus-visible:outline-2 focus-visible:outline-[#ff1f3d]" aria-label="Cover Compro, buka katalog Company Profile">
          <div class="aspect-[3/4] overflow-hidden bg-[#0c0c0d]">
            <svg viewBox="0 0 300 400" class="h-full w-full transition duration-500 group-hover:scale-105" preserveAspectRatio="xMidYMid slice" role="img" aria-label="Cover company profile" xmlns="http://www.w3.org/2000/svg">
            <rect width="300" height="400" fill="#262626"/>
            <rect x="46" y="34" width="208" height="332" rx="6" fill="#0A0A0A"/>
            <polygon points="46,230 254,160 254,366 46,366" fill="#FF1F3D"/>
            <circle cx="96" cy="92" r="20" fill="none" stroke="#FF1F3D" stroke-width="4"/><circle cx="96" cy="92" r="6" fill="#FF1F3D"/>
            <rect x="76" y="140" width="120" height="12" rx="6.0" fill="#fff"/><rect x="76" y="162" width="84" height="7" rx="3.5" fill="#fff" opacity="0.55"/><rect x="76" y="320" width="90" height="9" rx="4.5" fill="#0A0A0A"/>
          </svg>
          </div>
          <div class="pointer-events-none absolute inset-x-0 bottom-0 bg-gradient-to-t from-[#050505] to-transparent px-3 pb-3 pt-12">
            <p class="text-[10px] font-semibold uppercase tracking-wider text-[#ff6b7a]">Company Profile</p>
            <p class="text-base font-bold leading-tight text-white">Cover Compro</p>
          </div>
        </a>

        <a href="#katalog" data-gcat="undangan" class="gal reveal group relative block overflow-hidden rounded-2xl border border-white/10 transition hover:-translate-y-1 hover:border-[#ff1f3d]/40 focus-visible:outline focus-visible:outline-2 focus-visible:outline-[#ff1f3d]" aria-label="Undangan Ulang Tahun, buka katalog Undangan">
          <div class="aspect-[3/4] overflow-hidden bg-[#0c0c0d]">
            <svg viewBox="0 0 300 400" class="h-full w-full transition duration-500 group-hover:scale-105" preserveAspectRatio="xMidYMid slice" role="img" aria-label="Undangan ulang tahun" xmlns="http://www.w3.org/2000/svg">
            <rect width="300" height="400" fill="#FF1F3D"/>
            <circle cx="50" cy="60" r="9" fill="#0A0A0A"/><circle cx="256" cy="86" r="7" fill="#fff"/><circle cx="70" cy="330" r="7" fill="#fff"/><circle cx="252" cy="326" r="10" fill="#0A0A0A"/>
            <rect x="40" y="40" width="220" height="320" rx="16" fill="#fff"/>
            <path d="M110 166Q150 218 150 224M150 140Q150 190 150 224M190 166Q150 218 150 224" stroke="#0A0A0A" stroke-width="3" fill="none"/>
            <ellipse cx="110" cy="118" rx="26" ry="32" fill="#FF1F3D"/><ellipse cx="150" cy="100" rx="26" ry="32" fill="#0A0A0A"/><ellipse cx="190" cy="118" rx="26" ry="32" fill="#FF1F3D"/>
            <rect x="96" y="248" width="108" height="10" rx="5.0" fill="#0A0A0A"/><rect x="80" y="270" width="140" height="6" rx="3.0" fill="#0A0A0A" opacity="0.35"/><rect x="100" y="286" width="100" height="6" rx="3.0" fill="#0A0A0A" opacity="0.35"/><rect x="112" y="316" width="76" height="16" rx="8.0" fill="#FF1F3D"/>
          </svg>
          </div>
          <div class="pointer-events-none absolute inset-x-0 bottom-0 bg-gradient-to-t from-[#050505] to-transparent px-3 pb-3 pt-12">
            <p class="text-[10px] font-semibold uppercase tracking-wider text-[#ff6b7a]">Undangan</p>
            <p class="text-base font-bold leading-tight text-white">Undangan Ulang Tahun</p>
          </div>
        </a>

        <a href="#katalog" data-gcat="banner" class="gal reveal group relative block overflow-hidden rounded-2xl border border-white/10 transition hover:-translate-y-1 hover:border-[#ff1f3d]/40 focus-visible:outline focus-visible:outline-2 focus-visible:outline-[#ff1f3d]" aria-label="Banner Diskon, buka katalog Banner">
          <div class="aspect-[3/4] overflow-hidden bg-[#0c0c0d]">
            <svg viewBox="0 0 300 400" class="h-full w-full transition duration-500 group-hover:scale-105" preserveAspectRatio="xMidYMid slice" role="img" aria-label="Banner diskon" xmlns="http://www.w3.org/2000/svg">
            <rect width="300" height="400" fill="#FF1F3D"/>
            <rect x="28" y="28" width="244" height="344" rx="10" fill="none" stroke="#0A0A0A" stroke-width="3" stroke-dasharray="10 8"/>
            <text x="150" y="104" text-anchor="middle" font-family="Inter,Arial,sans-serif" font-size="26" font-weight="800" fill="#0A0A0A">DISKON</text>
            <text x="150" y="214" text-anchor="middle" font-family="Inter,Arial,sans-serif" font-size="100" font-weight="900" fill="#0A0A0A">50%</text>
            <rect x="86" y="252" width="128" height="10" rx="5.0" fill="#0A0A0A" opacity="0.6"/><rect x="100" y="272" width="100" height="10" rx="5.0" fill="#0A0A0A" opacity="0.6"/><rect x="96" y="316" width="108" height="22" rx="11.0" fill="#0A0A0A"/>
          </svg>
          </div>
          <div class="pointer-events-none absolute inset-x-0 bottom-0 bg-gradient-to-t from-[#050505] to-transparent px-3 pb-3 pt-12">
            <p class="text-[10px] font-semibold uppercase tracking-wider text-[#ff6b7a]">Banner</p>
            <p class="text-base font-bold leading-tight text-white">Banner Diskon</p>
          </div>
        </a>

        <a href="#katalog" data-gcat="logo" class="gal reveal group relative block overflow-hidden rounded-2xl border border-white/10 transition hover:-translate-y-1 hover:border-[#ff1f3d]/40 focus-visible:outline focus-visible:outline-2 focus-visible:outline-[#ff1f3d]" aria-label="Logo Kuliner, buka katalog Logo">
          <div class="aspect-[3/4] overflow-hidden bg-[#0c0c0d]">
            <svg viewBox="0 0 300 400" class="h-full w-full transition duration-500 group-hover:scale-105" preserveAspectRatio="xMidYMid slice" role="img" aria-label="Logo kuliner" xmlns="http://www.w3.org/2000/svg">
            <rect width="300" height="400" fill="#F2F2F2"/>
            <circle cx="150" cy="170" r="76" fill="#0A0A0A"/>
            <path d="M102 176h96a48 48 0 0 1-96 0z" fill="#FF1F3D"/>
            <path d="M128 160q-10-14 0-28M150 160q-10-14 0-28M172 160q-10-14 0-28" stroke="#fff" stroke-width="5" fill="none" stroke-linecap="round"/>
            <rect x="104" y="282" width="92" height="12" rx="6.0" fill="#0A0A0A"/><rect x="124" y="306" width="52" height="7" rx="3.5" fill="#0A0A0A" opacity="0.4"/>
          </svg>
          </div>
          <div class="pointer-events-none absolute inset-x-0 bottom-0 bg-gradient-to-t from-[#050505] to-transparent px-3 pb-3 pt-12">
            <p class="text-[10px] font-semibold uppercase tracking-wider text-[#ff6b7a]">Logo</p>
            <p class="text-base font-bold leading-tight text-white">Logo Kuliner</p>
          </div>
        </a>

        <a href="#katalog" data-gcat="compro" class="gal reveal group relative block overflow-hidden rounded-2xl border border-white/10 transition hover:-translate-y-1 hover:border-[#ff1f3d]/40 focus-visible:outline focus-visible:outline-2 focus-visible:outline-[#ff1f3d]" aria-label="Katalog Produk, buka katalog Company Profile">
          <div class="aspect-[3/4] overflow-hidden bg-[#0c0c0d]">
            <svg viewBox="0 0 300 400" class="h-full w-full transition duration-500 group-hover:scale-105" preserveAspectRatio="xMidYMid slice" role="img" aria-label="Katalog produk" xmlns="http://www.w3.org/2000/svg">
            <rect width="300" height="400" fill="#F2F2F2"/>
            <rect x="30" y="28" width="240" height="344" rx="6" fill="#fff"/>
            <rect x="52" y="50" width="100" height="10" rx="5.0" fill="#0A0A0A"/>
            <rect x="52" y="88" width="88" height="68" rx="4" fill="#0A0A0A"/>
            <rect x="52" y="164" width="60" height="7" rx="3.5" fill="#0A0A0A" opacity="0.45"/>
            <rect x="52" y="178" width="36" height="7" rx="3.5" fill="#FF1F3D"/>
            <rect x="160" y="88" width="88" height="68" rx="4" fill="#FF1F3D"/>
            <rect x="160" y="164" width="60" height="7" rx="3.5" fill="#0A0A0A" opacity="0.45"/>
            <rect x="160" y="178" width="36" height="7" rx="3.5" fill="#FF1F3D"/>
            <rect x="52" y="202" width="88" height="68" rx="4" fill="#FF1F3D"/>
            <rect x="52" y="278" width="60" height="7" rx="3.5" fill="#0A0A0A" opacity="0.45"/>
            <rect x="52" y="292" width="36" height="7" rx="3.5" fill="#FF1F3D"/>
            <rect x="160" y="202" width="88" height="68" rx="4" fill="#0A0A0A"/>
            <rect x="160" y="278" width="60" height="7" rx="3.5" fill="#0A0A0A" opacity="0.45"/>
            <rect x="160" y="292" width="36" height="7" rx="3.5" fill="#FF1F3D"/>
          </svg>
          </div>
          <div class="pointer-events-none absolute inset-x-0 bottom-0 bg-gradient-to-t from-[#050505] to-transparent px-3 pb-3 pt-12">
            <p class="text-[10px] font-semibold uppercase tracking-wider text-[#ff6b7a]">Company Profile</p>
            <p class="text-base font-bold leading-tight text-white">Katalog Produk</p>
          </div>
        </a>

        <a href="#katalog" data-gcat="undangan" class="gal reveal group relative block overflow-hidden rounded-2xl border border-white/10 transition hover:-translate-y-1 hover:border-[#ff1f3d]/40 focus-visible:outline focus-visible:outline-2 focus-visible:outline-[#ff1f3d]" aria-label="Undangan Syukuran, buka katalog Undangan">
          <div class="aspect-[3/4] overflow-hidden bg-[#0c0c0d]">
            <svg viewBox="0 0 300 400" class="h-full w-full transition duration-500 group-hover:scale-105" preserveAspectRatio="xMidYMid slice" role="img" aria-label="Undangan syukuran" xmlns="http://www.w3.org/2000/svg">
            <rect width="300" height="400" fill="#F5F5F5"/>
            <ellipse cx="62" cy="330" rx="18" ry="40" fill="#FF1F3D" opacity=".85" transform="rotate(-24 62 330)"/>
            <ellipse cx="238" cy="330" rx="18" ry="40" fill="#FF1F3D" opacity=".85" transform="rotate(24 238 330)"/>
            <path d="M60 376V150a90 90 0 0 1 180 0v226z" fill="#0A0A0A"/>
            <path d="M74 376V152a76 76 0 0 1 152 0v224z" fill="none" stroke="#FF1F3D" stroke-width="2"/>
            <circle cx="150" cy="140" r="18" fill="#FF1F3D"/>
            <rect x="112" y="196" width="76" height="9" rx="4.5" fill="#fff"/><rect x="94" y="218" width="112" height="6" rx="3.0" fill="#fff" opacity="0.55"/><rect x="102" y="234" width="96" height="6" rx="3.0" fill="#fff" opacity="0.55"/><rect x="118" y="276" width="64" height="16" rx="8.0" fill="#FF1F3D"/>
          </svg>
          </div>
          <div class="pointer-events-none absolute inset-x-0 bottom-0 bg-gradient-to-t from-[#050505] to-transparent px-3 pb-3 pt-12">
            <p class="text-[10px] font-semibold uppercase tracking-wider text-[#ff6b7a]">Undangan</p>
            <p class="text-base font-bold leading-tight text-white">Undangan Syukuran</p>
          </div>
        </a>

        <a href="#katalog" data-gcat="banner" class="gal reveal group relative block overflow-hidden rounded-2xl border border-white/10 transition hover:-translate-y-1 hover:border-[#ff1f3d]/40 focus-visible:outline focus-visible:outline-2 focus-visible:outline-[#ff1f3d]" aria-label="Grand Opening, buka katalog Banner">
          <div class="aspect-[3/4] overflow-hidden bg-[#0c0c0d]">
            <svg viewBox="0 0 300 400" class="h-full w-full transition duration-500 group-hover:scale-105" preserveAspectRatio="xMidYMid slice" role="img" aria-label="Banner grand opening" xmlns="http://www.w3.org/2000/svg">
            <rect width="300" height="400" fill="#0A0A0A"/>
            <circle cx="40" cy="40" r="6" fill="#FF1F3D"/><circle cx="262" cy="64" r="5" fill="#fff"/><circle cx="150" cy="30" r="4" fill="#FF1F3D"/>
            <rect x="24" y="84" width="252" height="232" rx="10" fill="none" stroke="#FF1F3D" stroke-width="3" stroke-dasharray="10 8"/>
            <text x="150" y="168" text-anchor="middle" font-family="Inter,Arial,sans-serif" font-size="48" font-weight="800" fill="#fff">GRAND</text>
            <text x="150" y="222" text-anchor="middle" font-family="Inter,Arial,sans-serif" font-size="48" font-weight="800" fill="#FF1F3D">OPENING</text>
            <rect x="96" y="252" width="108" height="9" rx="4.5" fill="#fff" opacity="0.5"/><rect x="112" y="276" width="76" height="9" rx="4.5" fill="#fff" opacity="0.35"/>
            <circle cx="262" cy="360" r="6" fill="#FF1F3D"/><circle cx="44" cy="352" r="5" fill="#fff"/>
          </svg>
          </div>
          <div class="pointer-events-none absolute inset-x-0 bottom-0 bg-gradient-to-t from-[#050505] to-transparent px-3 pb-3 pt-12">
            <p class="text-[10px] font-semibold uppercase tracking-wider text-[#ff6b7a]">Banner</p>
            <p class="text-base font-bold leading-tight text-white">Grand Opening</p>
          </div>
        </a>
      </div>
    </section>

    <!-- CARA KERJA -->
    <section id="cara-kerja" class="mx-auto max-w-6xl px-5 pt-24">
      <div class="reveal">
        <p class="text-sm font-semibold uppercase tracking-[.25em] text-[#ff6b7a]">Cara Kerja</p>
        <h2 class="mt-3 text-4xl font-semibold text-white sm:text-5xl">Empat Langkah Mudah</h2>
        <p class="mt-3 max-w-xl text-white/60">Dari ide sampai desain siap pakai.</p>
      </div>
      <ol id="steps" class="relative mt-14 grid gap-10 md:grid-cols-4 md:gap-6">
        <div class="absolute left-[12.5%] right-[12.5%] top-8 hidden h-0.5 -translate-y-1/2 bg-white/10 md:block" aria-hidden="true">
          <div class="step-line-h h-full bg-gradient-to-r from-[#ff1f3d] to-black"></div>
        </div>
        <li class="step relative flex gap-5 md:flex-col md:items-center md:text-center" style="--i:0">
          <span class="conn-v md:hidden" aria-hidden="true"></span>
          <div class="step-dot relative z-10 flex h-16 w-16 shrink-0 items-center justify-center rounded-full border border-[#ff1f3d]/40 bg-[#111112] text-[#ff6b7a] shadow-[0_0_24px_rgba(255,31,61,.2)] ring-4 ring-[#050505]">
            <svg class="step-icon h-7 w-7" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true"><path pathLength="1" d="M9 4h6a1 1 0 0 1 1 1v1H8V5a1 1 0 0 1 1-1z"/><path pathLength="1" d="M8 6H6a1 1 0 0 0-1 1v13a1 1 0 0 0 1 1h12a1 1 0 0 0 1-1V7a1 1 0 0 0-1-1h-2"/><path pathLength="1" d="M9 12h6M9 16h4"/></svg>
            <span class="absolute -right-1 -top-1 flex h-6 w-6 items-center justify-center rounded-full bg-gradient-to-br from-[#ff1f3d] to-black text-xs font-bold text-white">1</span>
          </div>
          <div class="pt-1 md:pt-0">
            <h3 class="text-xl font-semibold text-white">Brief</h3>
            <p class="mt-2 text-sm leading-relaxed text-white/60">Kita mulai dengan berbincang: kebutuhan, target audiens, ukuran, dan referensi desain yang kamu suka.</p>
          </div>
        </li>
        <li class="step relative flex gap-5 md:flex-col md:items-center md:text-center" style="--i:1">
          <span class="conn-v md:hidden" aria-hidden="true"></span>
          <div class="step-dot relative z-10 flex h-16 w-16 shrink-0 items-center justify-center rounded-full border border-[#ff1f3d]/40 bg-[#111112] text-[#ff6b7a] shadow-[0_0_24px_rgba(255,31,61,.2)] ring-4 ring-[#050505]">
            <svg class="step-icon h-7 w-7" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true"><path pathLength="1" d="M4 20l1-4L16 5l3 3L8 19z"/><path pathLength="1" d="M14 7l3 3"/></svg>
            <span class="absolute -right-1 -top-1 flex h-6 w-6 items-center justify-center rounded-full bg-gradient-to-br from-[#ff1f3d] to-black text-xs font-bold text-white">2</span>
          </div>
          <div class="pt-1 md:pt-0">
            <h3 class="text-xl font-semibold text-white">Sketsa</h3>
            <p class="mt-2 text-sm leading-relaxed text-white/60">Saya membuat sketsa dan konsep awal sebagai gambaran arah desain sebelum masuk ke tahap detail.</p>
          </div>
        </li>
        <li class="step relative flex gap-5 md:flex-col md:items-center md:text-center" style="--i:2">
          <span class="conn-v md:hidden" aria-hidden="true"></span>
          <div class="step-dot relative z-10 flex h-16 w-16 shrink-0 items-center justify-center rounded-full border border-[#ff1f3d]/40 bg-[#111112] text-[#ff6b7a] shadow-[0_0_24px_rgba(255,31,61,.2)] ring-4 ring-[#050505]">
            <svg class="step-icon h-7 w-7" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true"><path pathLength="1" d="M20 11a8 8 0 0 0-14.5-4.2L4 9"/><path pathLength="1" d="M4 4v5h5"/><path pathLength="1" d="M4 13a8 8 0 0 0 14.5 4.2L20 15"/><path pathLength="1" d="M20 20v-5h-5"/></svg>
            <span class="absolute -right-1 -top-1 flex h-6 w-6 items-center justify-center rounded-full bg-gradient-to-br from-[#ff1f3d] to-black text-xs font-bold text-white">3</span>
          </div>
          <div class="pt-1 md:pt-0">
            <h3 class="text-xl font-semibold text-white">Revisi</h3>
            <p class="mt-2 text-sm leading-relaxed text-white/60">Kamu memberi masukan, lalu saya sempurnakan desainnya sampai sesuai dengan yang diharapkan.</p>
          </div>
        </li>
        <li class="step relative flex gap-5 md:flex-col md:items-center md:text-center" style="--i:3">
          <div class="step-dot relative z-10 flex h-16 w-16 shrink-0 items-center justify-center rounded-full border border-[#ff1f3d]/40 bg-[#111112] text-[#ff6b7a] shadow-[0_0_24px_rgba(255,31,61,.2)] ring-4 ring-[#050505]">
            <svg class="step-icon h-7 w-7" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true"><circle pathLength="1" cx="12" cy="12" r="9"/><path pathLength="1" d="M8 12.5l2.7 2.7L16 9.5"/></svg>
            <span class="absolute -right-1 -top-1 flex h-6 w-6 items-center justify-center rounded-full bg-gradient-to-br from-[#ff1f3d] to-black text-xs font-bold text-white">4</span>
          </div>
          <div class="pt-1 md:pt-0">
            <h3 class="text-xl font-semibold text-white">Finishing</h3>
            <p class="mt-2 text-sm leading-relaxed text-white/60">Pemeriksaan akhir warna dan ukuran, lalu file siap cetak atau siap pakai diserahkan kepadamu.</p>
          </div>
        </li>
      </ol>
    </section>

    <!-- TENTANG -->
    <section id="tentang" class="mx-auto max-w-6xl px-5 pt-24">
      <div class="grid items-center gap-10 md:grid-cols-2">
        <figure class="reveal relative">
          <div class="absolute -inset-3 rounded-[2rem] bg-gradient-to-br from-[#ff1f3d]/25 to-black/25 blur-2xl"></div>
          <img src="data:image/jpeg;base64,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" alt="Meja kerja desainer dengan mikrofon dan monitor" class="relative aspect-square w-full rounded-[2rem] border border-white/10 object-cover" loading="lazy" />
        </figure>
        <div class="reveal">
          <p class="text-sm font-semibold uppercase tracking-[.25em] text-[#ff6b7a]">Tentang Saya</p>
          <h2 class="mt-3 text-4xl font-semibold text-white sm:text-5xl">Desainer Profesional</h2>
          <div class="mt-6 space-y-4 text-lg leading-relaxed text-white/60">
            <p>Saya Dede Wahyudi, desainer grafis profesional yang mengubah ide menjadi tampilan visual yang kuat, rapi, dan mudah diingat. Saya berpengalaman menangani branding, media promosi, hingga desain siap cetak, dengan perhatian penuh pada warna, tipografi, dan tata letak.</p>
            <p>Setiap proyek saya mulai dengan memahami kebutuhan klien dan target audiensnya. Hasil akhirnya tidak hanya enak dilihat, tetapi juga efektif menyampaikan pesan dan akurat saat naik cetak. Komunikasi yang jelas dan ketepatan waktu adalah prinsip kerja saya.</p>
          </div>
          <div class="mt-6 flex flex-wrap gap-2">
            <span class="rounded-full border border-white/10 bg-white/5 px-4 py-2 text-sm text-white">Desain Logo</span>
            <span class="rounded-full border border-white/10 bg-white/5 px-4 py-2 text-sm text-white">Branding</span>
            <span class="rounded-full border border-white/10 bg-white/5 px-4 py-2 text-sm text-white">Layout Cetak</span>
            <span class="rounded-full border border-white/10 bg-white/5 px-4 py-2 text-sm text-white">Banner &amp; Spanduk</span>
            <span class="rounded-full border border-white/10 bg-white/5 px-4 py-2 text-sm text-white">Tipografi</span>
            <span class="rounded-full border border-white/10 bg-white/5 px-4 py-2 text-sm text-white">Persiapan File Cetak</span>
          </div>
        </div>
      </div>
    </section>

    <!-- HUBUNG KAMI -->
    <section id="kontak" class="mx-auto max-w-6xl px-5 pt-24">
      <div class="reveal relative overflow-hidden rounded-[2rem] border border-white/10 bg-gradient-to-br from-[#3a0b12] via-[#0b0b0c] to-black px-6 py-16 text-center">
        <div class="pointer-events-none absolute -left-10 -top-10 h-56 w-56 rounded-full bg-[#ff1f3d]/20 blur-3xl"></div>
        <div class="pointer-events-none absolute -bottom-10 -right-10 h-56 w-56 rounded-full bg-[#ff1f3d]/10 blur-3xl"></div>
        <h2 class="relative text-4xl font-extrabold italic text-white sm:text-6xl">Hubung Kami</h2>
        <a href="https://wa.me/6281234567890?text=Halo%20Dede%2C%20saya%20tertarik%20dengan%20jasa%20desain%20Anda." target="_blank" rel="noopener noreferrer"
           class="relative mt-8 inline-flex items-center gap-3 rounded-full bg-[#25D366] px-8 py-4 text-lg font-semibold text-[#04210f] shadow-lg shadow-[#25D366]/30 transition hover:-translate-y-0.5 hover:shadow-xl focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-white">
          <svg class="h-6 w-6" viewBox="0 0 24 24" aria-hidden="true"><path d="M12 2a10 10 0 0 0-8.6 15.1L2 22l5-1.3A10 10 0 1 0 12 2z" fill="none" stroke="currentColor" stroke-width="2" stroke-linejoin="round"/><path d="M8.5 8.5c0 3.5 3.5 7 7 7l1.2-1.6-2.2-1.4-1 .8c-1-.5-1.8-1.3-2.3-2.3l.8-1-1.4-2.2z" fill="currentColor"/></svg>
          WhatsApp
        </a>
      </div>
    </section>
  </main>

  <footer class="mx-auto mt-24 max-w-6xl border-t border-white/10 px-5 py-8 text-center text-sm text-white/40">
    © <span id="year"></span> Dede Wahyudi. Jasa desain logo, undangan, banner, dan company profile.
  </footer>

  <!-- Toast -->
  <div id="toast" role="status" aria-live="polite" class="pointer-events-none fixed inset-x-0 bottom-6 z-[70] flex justify-center px-4 opacity-0 transition-opacity duration-300">
    <span id="toastText" class="rounded-full border border-[#ff1f3d]/40 bg-[#111112] px-5 py-3 text-sm font-medium text-white shadow-xl"></span>
  </div>

  <!-- Detail desain -->
  <div id="modal" class="fixed inset-0 z-[60] hidden items-end justify-center sm:items-center sm:p-4" role="dialog" aria-modal="true" aria-labelledby="mTitle">
    <div data-close class="absolute inset-0 bg-black/80 backdrop-blur-sm"></div>
    <div class="relative flex max-h-[92vh] w-full max-w-3xl flex-col overflow-hidden rounded-t-[2rem] border border-white/10 bg-[#0b0b0c] shadow-2xl sm:rounded-[2rem]">
      <button type="button" data-close id="mClose" aria-label="Tutup" class="absolute right-3 top-3 z-10 flex h-10 w-10 items-center justify-center rounded-full bg-black/70 text-white backdrop-blur transition hover:bg-[#ff1f3d] hover:text-white">
        <svg class="h-5 w-5" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" viewBox="0 0 24 24"><path d="M6 6l12 12M18 6L6 18"/></svg>
      </button>
      <div class="overflow-y-auto">
        <div id="mMedia" class="aspect-[4/3] w-full overflow-hidden bg-[#0c0c0d]"></div>
        <div class="p-6 sm:p-8">
          <p id="mCount" class="text-xs font-semibold uppercase tracking-[.2em] text-[#ff6b7a]"></p>
          <h2 id="mTitle" class="mt-2 text-3xl font-semibold text-white"></h2>
          <p id="mTags" class="mt-1 text-sm font-medium text-white/50"></p>
          <p id="mDesc" class="mt-4 leading-relaxed text-white/60"></p>
          <p id="mPrice" class="mt-4 text-2xl font-bold text-[#ff4d5e]"></p>
          <div class="mt-6 flex flex-wrap items-center justify-between gap-3">
            <div class="flex gap-2">
              <button id="mPrev" type="button" class="rounded-full border border-white/15 px-4 py-2.5 text-sm font-medium text-white transition hover:border-[#ff1f3d]/60">&larr; Sebelumnya</button>
              <button id="mNext" type="button" class="rounded-full border border-white/15 px-4 py-2.5 text-sm font-medium text-white transition hover:border-[#ff1f3d]/60">Berikutnya &rarr;</button>
            </div>
            <button id="mAdd" type="button" class="grad-btn rounded-full px-6 py-3 font-semibold">Tambah ke Pesanan</button>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- Pesanan -->
  <div id="drawer" class="fixed inset-0 z-[60] hidden items-end justify-center sm:items-center sm:p-4" role="dialog" aria-modal="true" aria-labelledby="dTitle">
    <div data-close class="absolute inset-0 bg-black/80 backdrop-blur-sm"></div>
    <div class="relative flex max-h-[88vh] w-full max-w-xl flex-col overflow-hidden rounded-t-[2rem] border border-white/10 bg-[#0b0b0c] shadow-2xl sm:rounded-[2rem]">
      <div class="flex items-center justify-between border-b border-white/10 px-6 py-5">
        <h2 id="dTitle" class="text-2xl font-semibold text-white">Pesanan Saya</h2>
        <button type="button" data-close id="dClose" aria-label="Tutup" class="flex h-10 w-10 items-center justify-center rounded-full text-white transition hover:bg-white/10">
          <svg class="h-5 w-5" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" viewBox="0 0 24 24"><path d="M6 6l12 12M18 6L6 18"/></svg>
        </button>
      </div>
      <div id="dList" class="flex-1 space-y-3 overflow-y-auto px-6 py-5"></div>
      <div id="dEmpty" class="hidden px-6 py-10 text-center">
        <p class="text-white/60">Pesananmu masih kosong. Pilih desain di katalog, lalu tambahkan ke pesanan.</p>
        <a href="#katalog" data-close class="grad-btn mt-6 inline-flex rounded-full px-6 py-3 font-semibold">Lihat Katalog</a>
      </div>
      <div id="dFoot" class="border-t border-white/10 px-6 py-5">
        <div class="flex items-center justify-between text-lg">
          <span class="text-white/60">Perkiraan total</span>
          <span id="dTotal" class="font-bold text-[#ff4d5e]"></span>
        </div>
        <p class="mt-1 text-xs text-white/40">Harga awal bersifat perkiraan. Harga akhir disepakati lewat WhatsApp.</p>
        <button id="dSend" type="button" class="mt-4 flex w-full items-center justify-center gap-3 rounded-full bg-[#25D366] px-6 py-4 text-lg font-semibold text-[#04210f] transition hover:-translate-y-0.5">
          Kirim Pesanan via WhatsApp
        </button>
        <button id="dClear" type="button" class="mt-3 w-full text-center text-sm text-white/50 underline-offset-4 hover:text-white hover:underline">Kosongkan pesanan</button>
      </div>
    </div>
  </div>

  <script>
    (function () {
      'use strict';
      var $ = function (s, r) { return (r || document).querySelector(s); };
      var $$ = function (s, r) { return Array.prototype.slice.call((r || document).querySelectorAll(s)); };
      var rupiah = function (n) { return 'Rp ' + Number(n).toLocaleString('id-ID'); };
      var WA_NUMBER = '6281234567890'; // ganti dengan nomor WhatsApp (kode negara, tanpa + atau 0 di depan)
      var reduce = window.matchMedia('(prefers-reduced-motion: reduce)').matches;
      var store = {
        get: function (k, d) { try { var v = localStorage.getItem(k); return v ? JSON.parse(v) : d; } catch (e) { return d; } },
        set: function (k, v) { try { localStorage.setItem(k, JSON.stringify(v)); } catch (e) {} }
      };
      var CAT_LABEL = { undangan: 'Undangan', banner: 'Banner', logo: 'Logo', compro: 'Company Profile' };

      $('#year').textContent = new Date().getFullYear();

      /* ---------- Data katalog ---------- */
      var catalogCards = $$('#catalogGrid .card');
      var ITEMS = catalogCards.map(function (c) {
        return { id: c.dataset.id, cat: c.dataset.cat, title: c.dataset.title, desc: c.dataset.desc,
                 tags: c.dataset.tags, price: Number(c.dataset.price), svg: c.querySelector('svg') };
      });
      var byId = {};
      ITEMS.forEach(function (i) { byId[i.id] = i; });
      function cloneSvg(it, cls) {
        var s = it.svg.cloneNode(true);
        s.setAttribute('class', cls || 'h-full w-full');
        return s;
      }

      /* ---------- Header: tinggi, tab, scroll-spy ---------- */
      var topbar = $('#topbar');
      function setHH() { document.documentElement.style.setProperty('--hh', topbar.offsetHeight + 'px'); }
      setHH();
      window.addEventListener('resize', setHH);
      if (document.fonts && document.fonts.ready) document.fonts.ready.then(setHH);

      var tabs = $$('#tabs .tab');
      var tabNav = $('#tabs');
      var targets = tabs.map(function (a) { return $(a.getAttribute('href')); });
      var curTab = -1;
      function spy() {
        var y = topbar.offsetHeight + 60, cur = 0;
        targets.forEach(function (t, i) { if (t && t.getBoundingClientRect().top <= y) cur = i; });
        if (window.innerHeight + window.scrollY >= document.documentElement.scrollHeight - 4) cur = tabs.length - 1;
        if (cur === curTab) return;
        curTab = cur;
        tabs.forEach(function (a, i) { a.classList.toggle('active', i === cur); });
        var a = tabs[cur];
        tabNav.scrollTo({ left: a.offsetLeft - tabNav.clientWidth / 2 + a.clientWidth / 2, behavior: reduce ? 'auto' : 'smooth' });
      }
      window.addEventListener('scroll', spy, { passive: true });
      spy();

      /* ---------- Reveal & hitung angka ---------- */
      var rio = ('IntersectionObserver' in window) ? new IntersectionObserver(function (es) {
        es.forEach(function (e) { if (e.isIntersecting) { e.target.classList.add('show'); rio.unobserve(e.target); } });
      }, { threshold: 0.12 }) : null;
      $$('.reveal').forEach(function (el) { rio ? rio.observe(el) : el.classList.add('show'); });

      function animateCounter(el) {
        var target = parseInt(el.dataset.target, 10), dur = 1800, t0 = performance.now();
        (function frame(now) {
          var t = Math.min((now - t0) / dur, 1);
          el.textContent = Math.round(target * (1 - Math.pow(1 - t, 3)));
          if (t < 1) requestAnimationFrame(frame);
        })(t0);
      }
      if (!reduce && rio) {
        var cio = new IntersectionObserver(function (es) {
          es.forEach(function (e) { if (e.isIntersecting) { animateCounter(e.target); cio.unobserve(e.target); } });
        }, { threshold: 0.6 });
        $$('.counter').forEach(function (el) { el.textContent = '0'; cio.observe(el); });
      }

      /* ---------- Cara kerja ---------- */
      var stepsEl = $('#steps');
      if ('IntersectionObserver' in window) {
        new IntersectionObserver(function (es) {
          es.forEach(function (e) { stepsEl.classList.toggle('steps-play', e.isIntersecting); });
        }, { threshold: 0.35 }).observe(stepsEl);
      } else { stepsEl.classList.add('steps-play'); }

      /* ---------- Cari & filter ---------- */
      var q = $('#q'), chips = $$('#chips .chip'), activeCat = 'all';
      function applyFilter() {
        var term = q.value.trim().toLowerCase(), n = 0;
        catalogCards.forEach(function (c) {
          var ok = (activeCat === 'all' || c.dataset.cat === activeCat) && (!term || c.dataset.search.indexOf(term) > -1);
          c.classList.toggle('hidden', !ok);
          if (ok) n++;
        });
        $('#emptyMsg').classList.toggle('hidden', n > 0);
        $('#resultCount').textContent = n + ' desain';
      }
      function setCat(cat) {
        activeCat = cat;
        chips.forEach(function (b) { b.classList.toggle('active', b.dataset.cat === cat); });
        applyFilter();
      }
      chips.forEach(function (b) { b.addEventListener('click', function () { setCat(b.dataset.cat); }); });
      q.addEventListener('input', applyFilter);
      $('#searchForm').addEventListener('submit', function (e) {
        e.preventDefault();
        applyFilter();
        $('#katalog').scrollIntoView({ behavior: reduce ? 'auto' : 'smooth' });
        q.blur();
      });
      $$('.gal').forEach(function (a) {
        a.addEventListener('click', function (e) {
          e.preventDefault();
          q.value = '';
          setCat(a.dataset.gcat);
          $('#katalog').scrollIntoView({ behavior: reduce ? 'auto' : 'smooth' });
        });
      });
      setCat('all');

      /* ---------- Toast ---------- */
      var toastT;
      function toast(msg) {
        $('#toastText').textContent = msg;
        var t = $('#toast');
        t.style.opacity = '1';
        clearTimeout(toastT);
        toastT = setTimeout(function () { t.style.opacity = '0'; }, 1800);
      }

      /* ---------- Pesanan (keranjang) ---------- */
      var cart = store.get('cart', {});
      Object.keys(cart).forEach(function (id) { if (!byId[id] || !(cart[id] > 0)) delete cart[id]; });
      function cartCount() { return Object.keys(cart).reduce(function (s, id) { return s + cart[id]; }, 0); }
      function cartTotal() { return Object.keys(cart).reduce(function (s, id) { return s + byId[id].price * cart[id]; }, 0); }

      function renderCart() {
        var n = cartCount(), total = cartTotal();

        var list = $('#dList');
        list.textContent = '';
        var ids = Object.keys(cart);
        $('#dEmpty').classList.toggle('hidden', ids.length > 0);
        list.classList.toggle('hidden', ids.length === 0);
        $('#dFoot').classList.toggle('hidden', ids.length === 0);
        ids.forEach(function (id) {
          var it = byId[id];
          var row = document.createElement('div');
          row.className = 'flex items-center gap-4 rounded-2xl border border-white/10 bg-white/5 p-3';
          var th = document.createElement('div');
          th.className = 'h-16 w-20 shrink-0 overflow-hidden rounded-xl bg-[#0c0c0d]';
          th.appendChild(cloneSvg(it));
          var info = document.createElement('div');
          info.className = 'min-w-0 flex-1';
          var t = document.createElement('p'); t.className = 'truncate font-semibold text-white'; t.textContent = it.title;
          var p = document.createElement('p'); p.className = 'text-sm text-[#ff4d5e]'; p.textContent = rupiah(it.price);
          info.appendChild(t); info.appendChild(p);
          var ctr = document.createElement('div');
          ctr.className = 'flex items-center gap-2';
          function btn(label, txt, fn) {
            var b = document.createElement('button');
            b.type = 'button'; b.setAttribute('aria-label', label); b.textContent = txt;
            b.className = 'flex h-9 w-9 items-center justify-center rounded-full border border-white/15 text-lg text-white transition hover:border-[#ff1f3d]/60';
            b.addEventListener('click', fn); return b;
          }
          var qty = document.createElement('span'); qty.className = 'w-6 text-center font-semibold text-white'; qty.textContent = cart[id];
          ctr.appendChild(btn('Kurangi ' + it.title, '−', function () { changeQty(id, -1); }));
          ctr.appendChild(qty);
          ctr.appendChild(btn('Tambah ' + it.title, '+', function () { changeQty(id, 1); }));
          row.appendChild(th); row.appendChild(info); row.appendChild(ctr);
          list.appendChild(row);
        });
        $('#dTotal').textContent = rupiah(total);
      }
      function saveCart() { store.set('cart', cart); renderCart(); }
      function addToCart(id) {
        cart[id] = (cart[id] || 0) + 1;
        saveCart();
        toast('Ditambahkan: ' + byId[id].title);
      }
      function changeQty(id, d) {
        cart[id] = (cart[id] || 0) + d;
        if (cart[id] <= 0) delete cart[id];
        saveCart();
      }
      $('#dClear').addEventListener('click', function () { cart = {}; saveCart(); });
      $('#dSend').addEventListener('click', function () {
        var lines = ['Halo Dede, saya ingin memesan desain:', ''];
        Object.keys(cart).forEach(function (id, i) {
          lines.push((i + 1) + '. ' + byId[id].title + ' x' + cart[id] + ' (mulai ' + rupiah(byId[id].price * cart[id]) + ')');
        });
        lines.push('', 'Perkiraan total: ' + rupiah(cartTotal()), 'Mohon info detail dan harga akhirnya. Terima kasih.');
        window.open('https://wa.me/' + WA_NUMBER + '?text=' + encodeURIComponent(lines.join('\n')), '_blank', 'noopener');
      });

      /* ---------- Dialog (modal & pesanan) ---------- */
      var lastFocus = null;
      function openDialog(el, focusSel) {
        lastFocus = document.activeElement;
        el.classList.remove('hidden'); el.classList.add('flex');
        document.body.style.overflow = 'hidden';
        var f = $(focusSel, el); if (f) f.focus();
      }
      function closeDialog(el) {
        if (el.classList.contains('hidden')) return;
        el.classList.add('hidden'); el.classList.remove('flex');
        if (!$('#modal').classList.contains('flex') && !$('#drawer').classList.contains('flex')) document.body.style.overflow = '';
        if (lastFocus && document.contains(lastFocus)) lastFocus.focus();
      }
      ['#modal', '#drawer'].forEach(function (sel) {
        var el = $(sel);
        $$('[data-close]', el).forEach(function (b) { b.addEventListener('click', function () { closeDialog(el); }); });
      });

      function openCart() { renderCart(); openDialog($('#drawer'), '#dClose'); }

      /* ---------- Detail desain ---------- */
      var mIdx = 0;
      function fillModal() {
        var it = ITEMS[mIdx];
        $('#mMedia').textContent = '';
        $('#mMedia').appendChild(cloneSvg(it));
        $('#mTitle').textContent = it.title;
        $('#mTags').textContent = it.tags;
        $('#mDesc').textContent = it.desc;
        $('#mPrice').textContent = 'Mulai ' + rupiah(it.price);
        $('#mCount').textContent = CAT_LABEL[it.cat] + ' • ' + (mIdx + 1) + ' dari ' + ITEMS.length;
      }
      function openItem(id) {
        mIdx = ITEMS.indexOf(byId[id]);
        fillModal();
        openDialog($('#modal'), '#mClose');
      }
      function stepModal(d) { mIdx = (mIdx + d + ITEMS.length) % ITEMS.length; fillModal(); }
      $('#mPrev').addEventListener('click', function () { stepModal(-1); });
      $('#mNext').addEventListener('click', function () { stepModal(1); });
      $('#mAdd').addEventListener('click', function () { addToCart(ITEMS[mIdx].id); });

      // Klik kartu (katalog & unggulan): tambah ke pesanan atau buka detail
      document.addEventListener('click', function (e) {
        var card = e.target.closest('.card');
        if (!card) return;
        if (e.target.closest('[data-add]')) { addToCart(card.dataset.id); return; }
        openItem(card.dataset.id);
      });

      document.addEventListener('keydown', function (e) {
        var modal = $('#modal'), drawer = $('#drawer');
        var openEl = modal.classList.contains('flex') ? modal : (drawer.classList.contains('flex') ? drawer : null);
        if (!openEl) return;
        if (e.key === 'Escape') { closeDialog(openEl); return; }
        if (openEl === modal && e.key === 'ArrowLeft') stepModal(-1);
        if (openEl === modal && e.key === 'ArrowRight') stepModal(1);
        if (e.key === 'Tab') {
          var f = $$('button, a[href]', openEl).filter(function (x) { return x.offsetParent !== null; });
          if (!f.length) return;
          var first = f[0], last = f[f.length - 1];
          if (e.shiftKey && document.activeElement === first) { e.preventDefault(); last.focus(); }
          else if (!e.shiftKey && document.activeElement === last) { e.preventDefault(); first.focus(); }
        }
      });

      /* ---------- Desain unggulan (grid) ---------- */
      ['l1', 'u1', 'c1', 'b1'].forEach(function (id) {
        var src = catalogCards.filter(function (c) { return c.dataset.id === id; })[0];
        if (src) $('#featGrid').appendChild(src.cloneNode(true));
      });

      /* ---------- Karya pilihan (carousel otomatis) ---------- */
      var FEAT = ['u1', 'b1', 'l1', 'c1', 'u2', 'l2'];
      var fi = 0, elapsed = 0, DUR = 5000, TICK = 100, paused = reduce;
      function renderFeat() {
        var it = byId[FEAT[fi]];
        $('#featSvg').textContent = '';
        $('#featSvg').appendChild(cloneSvg(it));
        $('#featLabel').textContent = 'Karya Pilihan • ' + (fi + 1) + ' / ' + FEAT.length;
        $('#featCat').textContent = CAT_LABEL[it.cat];
        $('#featTitle').textContent = it.title;
        $('#featDesc').textContent = it.desc;
        $('#featPrice').textContent = 'Mulai ' + rupiah(it.price);
        elapsed = 0; updateBar();
      }
      function updateBar() {
        $('#featBar').style.width = Math.min(elapsed / DUR * 100, 100) + '%';
        $('#featCount').textContent = paused ? 'Dijeda' : 'Ganti otomatis dalam ' + Math.max((DUR - elapsed) / 1000, 0).toFixed(1) + ' detik';
      }
      function featStep(d) { fi = (fi + d + FEAT.length) % FEAT.length; renderFeat(); }
      function setPaused(p) {
        paused = p;
        $('#featPauseText').textContent = p ? 'Putar' : 'Jeda';
        $('#icoPause').classList.toggle('hidden', p);
        $('#icoPlay').classList.toggle('hidden', !p);
        updateBar();
      }
      $('#featPause').addEventListener('click', function () { setPaused(!paused); });
      $('#featPrev').addEventListener('click', function () { featStep(-1); });
      $('#featNext').addEventListener('click', function () { featStep(1); });
      $('#featAdd').addEventListener('click', function () { addToCart(FEAT[fi]); });
      $('#featMedia').addEventListener('click', function () { openItem(FEAT[fi]); });
      setInterval(function () {
        if (paused || document.hidden) return;
        elapsed += TICK;
        if (elapsed >= DUR) featStep(1); else updateBar();
      }, TICK);
      renderFeat();
      setPaused(paused);

      renderCart();
    })();
  </script>
</body>
</html>
