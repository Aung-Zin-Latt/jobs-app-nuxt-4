<template>
  <section class="text-center">
    <p class="mb-4 inline-flex rounded-full border border-emerald-500/30 bg-emerald-500/10 px-3 py-1 text-xs font-medium text-emerald-400">
      Environment OK
    </p>
    <h1 class="text-4xl font-bold tracking-tight text-white sm:text-5xl">
      Welcome to Nuxt&nbsp;4
    </h1>
    <p class="mx-auto mt-4 max-w-xl text-lg text-slate-400">
      Tailwind CSS is working — this hero uses utilities only (no bespoke CSS blocks needed for layout).
      You are on Vue&nbsp;{{ vueMajor }} with the Composition API via
      <code class="rounded bg-slate-800 px-1.5 py-0.5 text-xs text-slate-300">&lt;script setup&gt;</code>.
    </p>
    <div class="mx-auto mt-10 flex flex-wrap items-center justify-center gap-3">
      <span class="rounded-lg bg-slate-800 px-4 py-2 text-sm font-medium text-slate-200 ring-1 ring-slate-700">
        Nuxt {{ nuxtMajor }}
      </span>
      <span class="rounded-lg bg-emerald-950 px-4 py-2 text-sm font-medium text-emerald-300 ring-1 ring-emerald-800">
        Tailwind 4 ✓
      </span>
      <span class="rounded-lg bg-slate-800 px-4 py-2 text-sm font-medium text-slate-200 ring-1 ring-slate-700">
        Vue {{ vueMajor }}
      </span>
    </div>
  </section>
</template>

<script setup>
import { version as vueFullVersion } from 'vue'

const vueMajor = vueFullVersion.startsWith('v')
  ? vueFullVersion.slice(1).split('.')[0]
  : vueFullVersion.split('.')[0]
const nuxtMajor = '4'
</script>
