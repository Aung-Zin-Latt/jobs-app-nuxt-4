<template>
  <div class="min-h-screen flex flex-col bg-slate-950 text-slate-100">

    <header class="border-b border-slate-800/80 bg-slate-900/80 backdrop-blur-md">
      <div class="mx-auto flex max-w-5xl items-center justify-between gap-4 px-4 py-3 sm:px-6">
        <NuxtLink
          to="/"
          class="text-sm font-semibold tracking-tight text-white hover:text-emerald-400/90 transition-colors"
        >
          App
        </NuxtLink>
        <span class="hidden text-xs text-slate-500 sm:inline">Nuxt 4 · Vue 3 · Tailwind 4</span>
      </div>
    </header>

    <main class="flex-1">
      <slot />
    </main>

    <footer class="border-t border-slate-800/80 py-4 text-center text-xs text-slate-600">
      Nuxt 4 baseline · extend as needed during feature work.
    </footer>
    
  </div>
</template>