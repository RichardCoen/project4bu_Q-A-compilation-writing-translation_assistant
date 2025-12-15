<script setup lang="ts">
import { Globe } from 'lucide-vue-next';
</script>

<template>
  <nav class="sticky top-0 z-50 w-full border-b border-white/10 bg-slate-950/80 backdrop-blur-md">
    <div class="container mx-auto flex h-16 items-center justify-between px-4">
      <div class="flex items-center gap-2">
        <div class="flex h-8 w-8 items-center justify-center rounded-lg bg-cyan-500/20 text-cyan-400">
          <Globe class="h-5 w-5" />
        </div>
        <span class="text-lg font-bold tracking-tight text-white">Translation Assistant</span>
      </div>
      
      <div class="hidden items-center gap-6 md:flex">
        <a href="#" class="text-sm font-medium text-slate-400 transition-colors hover:text-cyan-400">Product</a>
        <a href="#" class="text-sm font-medium text-slate-400 transition-colors hover:text-cyan-400">Pricing</a>
        <a href="#" class="text-sm font-medium text-slate-400 transition-colors hover:text-cyan-400">Resources</a>
      </div>

      <div class="flex items-center gap-4">
        <button class="text-sm font-medium text-slate-300 hover:text-white">Log in</button>
        <button class="rounded-full bg-cyan-500 px-4 py-2 text-sm font-medium text-white shadow-lg shadow-cyan-500/20 transition-all hover:bg-cyan-400 hover:shadow-cyan-500/40">
          Start Trial
        </button>
      </div>
    </div>
  </nav>
</template>
