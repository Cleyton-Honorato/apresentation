---
theme: default
title: Apresentação Academe
info: |
  ## Apresentação Academe
  Template com a identidade visual da Academe.
class: text-center academe-light
colorSchema: light
drawings:
  persist: false
transition: slide-left
mdc: true
# Fontes da marca (importadas automaticamente do Google Fonts)
fonts:
  sans: Plus Jakarta Sans
  serif: Sora
  weights: '400,500,600,700,800'
# CSS global com a paleta Academe
---

<!-- ============================================================
     CAPA
     ============================================================ -->

<AcademeDots />

<AcademeLogo variant="full-black" class="absolute top-8 left-1/2 -translate-x-1/2 h-12 z-10" />

<div class="relative flex flex-col items-center justify-center h-full">

  # <span style="color: var(--academe-primary)">ACATECH</span>

  <strong class="text-xl mt-2" style="color: var(--academe-bg)">Do PNG para sua máquina</strong>
</div>

<!--
Notas do apresentador ficam no último bloco de comentário do slide.
-->

---
class: academe-light
---

<div class="absolute inset-0 flex text-center">

  <!-- Lado esquerdo: Backoffice -->
  <div class="flex-1 flex flex-col items-center justify-center gap-3 px-16"
       style="background: linear-gradient(135deg, rgba(137,44,221,.08), rgba(168,85,247,.03))">
    <div class="text-sm font-semibold tracking-widest uppercase" style="color: var(--academe-primary)">Gestão interna</div>
    <h1 class="academe-gradient">Backoffice</h1>
    <div class="flex gap-4 mt-4">
      <div class="icon-chip"><carbon:settings /></div>
      <div class="icon-chip"><carbon:data-base /></div>
      <div class="icon-chip"><carbon:user-admin /></div>
    </div>
  </div>

  <!-- Lado direito: Portal -->
  <div class="flex-1 flex flex-col items-center justify-center gap-3 px-16">
    <div class="text-sm font-semibold tracking-widest uppercase" style="color: var(--academe-primary-light)">Dash, Portal e Escolas para o dia a dia</div>
    <h1 class="academe-gradient">Dash</h1>
    <div class="flex gap-4 mt-4">
      <div class="icon-chip"><carbon:dashboard /></div>
      <div class="icon-chip"><carbon:chart-line /></div>
      <div class="icon-chip"><carbon:screen /></div>
    </div>
  </div>

</div>

<!-- Divisória vertical central -->
<div class="absolute top-[15%] bottom-[15%] left-1/2 -translate-x-1/2 w-px"
     style="background: linear-gradient(180deg, transparent, rgba(137,44,221,.35), transparent)"></div>

<!-- Badge VS no centro -->
<div class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 flex items-center justify-center rounded-full"
     style="width:96px;height:96px;background:linear-gradient(135deg,#a855f7,#892cdd,#6b1fb8);box-shadow:0 12px 30px rgba(137,44,221,.4);border:4px solid #fff">
  <span class="font-bold text-white" style="font-family:'Sora';font-size:1.9rem;letter-spacing:.02em">VS</span>
</div>

<AcademeFooter />

---
layout: center
class: text-center academe-light
---

<AcademeDots variant="b" />

<div class="relative flex flex-col items-center justify-center gap-6">

  <div class="relative flex items-center justify-center">
    <div class="academe-ping" style="width:120px;height:120px"></div>
    <div class="academe-ping" style="width:120px;height:120px;animation-delay:1.3s"></div>
    <div class="relative flex items-center justify-center rounded-full text-white"
         style="width:120px;height:120px;background:linear-gradient(135deg,#a855f7,#892cdd,#6b1fb8);border:4px solid #fff;box-shadow:0 14px 34px rgba(137,44,221,.4);font-size:3.2rem;animation:academe-glow-pulse 3s ease-in-out infinite">
      <carbon:rocket />
    </div>
  </div>

  <h1 class="academe-gradient" style="font-size:3.4rem">Vamos à prática!</h1>
  <p class="text-xl" style="color:#555">Mão na massa — hora de colocar em prática</p>

</div>

<AcademeFooter />
