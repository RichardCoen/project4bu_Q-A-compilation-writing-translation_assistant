<script setup lang="ts">
import { ScanLine, BookType, ShieldCheck, Download, Lock, ChevronRight } from 'lucide-vue-next';

const features = [
  {
    icon: ScanLine,
    title: 'OCR & Parsing',
    description: 'High-precision layout recovery',
  },
  {
    icon: BookType,
    title: 'Terminology',
    description: 'Domain-specific consistency',
  },
  {
    icon: ShieldCheck,
    title: 'Quality Check',
    description: 'Automated proofreading & scores',
  },
  {
    icon: Download,
    title: 'Smart Export',
    description: 'Bilingual & format retention',
  },
  {
    icon: Lock,
    title: 'Security',
    description: 'Enterprise-grade permission',
  },
];
</script>

<template>
  <section class="bg-slate-900/50 py-24">
    <div class="container mx-auto px-4">
      <div class="mb-12 text-center">
        <h2 class="text-3xl font-bold text-white">Powerful Toolkit</h2>
        <p class="mt-4 text-slate-400">Everything you need for professional translation</p>
      </div>
      
      <div class="grid gap-6 sm:grid-cols-2 lg:grid-cols-3">
        <button
          v-for="feature in features"
          :key="feature.title"
          class="group relative flex flex-col overflow-hidden rounded-2xl border border-white/5 bg-slate-950 p-8 text-left transition-all hover:border-cyan-500/50 hover:bg-slate-900 hover:shadow-2xl hover:shadow-cyan-500/10"
        >
          <div class="mb-6 inline-flex h-12 w-12 items-center justify-center rounded-xl bg-slate-900 text-cyan-400 transition-colors group-hover:bg-cyan-500 group-hover:text-white">
            <component :is="feature.icon" class="h-6 w-6" />
          </div>
          
          <h3 class="text-xl font-bold text-white">{{ feature.title }}</h3>
          <p class="mt-2 text-sm text-slate-400">{{ feature.description }}</p>
          
          <div class="mt-6 flex items-center text-sm font-medium text-cyan-400 opacity-0 transition-opacity group-hover:opacity-100">
            <span>Launch Tool</span>
            <ChevronRight class="ml-1 h-4 w-4" />
          </div>
          
          <!-- Hover Gradient -->
          <div class="absolute inset-0 -z-10 bg-gradient-to-br from-cyan-500/5 via-transparent to-transparent opacity-0 transition-opacity group-hover:opacity-100"></div>
        </button>
      </div>
    </div>
  </section>
</template>
