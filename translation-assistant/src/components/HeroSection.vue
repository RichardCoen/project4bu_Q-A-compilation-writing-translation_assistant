<script setup lang="ts">
import { FileText, Mic, ArrowRight } from 'lucide-vue-next';
</script>

<template>
  <section class="relative overflow-hidden pt-20 pb-32">
    <!-- Background Effects -->
    <div class="absolute -top-24 -left-24 h-96 w-96 rounded-full bg-cyan-500/10 blur-3xl"></div>
    <div class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 h-[500px] w-[500px] rounded-full bg-blue-600/10 blur-[100px]"></div>
    
    <div class="container relative mx-auto px-4 text-center">
      <div class="inline-flex items-center gap-2 rounded-full border border-white/10 bg-white/5 px-3 py-1 text-xs font-medium text-cyan-400 backdrop-blur-sm">
        <span class="flex h-2 w-2 rounded-full bg-cyan-400"></span>
        Next Gen AI Translation
      </div>
      
      <h1 class="mt-8 text-5xl font-extrabold tracking-tight text-white sm:text-6xl lg:text-7xl">
        Translation <span class="bg-gradient-to-r from-cyan-400 to-blue-500 bg-clip-text text-transparent">Reimagined</span>
      </h1>
      
      <p class="mx-auto mt-6 max-w-2xl text-lg text-slate-400">
        Format fidelity, terminology consistency, and real-time efficiency. 
        The ultimate workspace for seamless cross-language communication.
      </p>
      
      <div class="mt-12 flex flex-col items-center justify-center gap-4 sm:flex-row">
        <button class="group relative flex h-16 w-full max-w-xs items-center justify-center gap-3 rounded-2xl bg-cyan-500 px-8 text-lg font-bold text-white shadow-xl shadow-cyan-500/20 transition-all hover:scale-105 hover:bg-cyan-400 hover:shadow-cyan-500/40 sm:w-auto">
          <FileText class="h-6 w-6" />
          <span>Upload Document</span>
          <ArrowRight class="h-5 w-5 opacity-0 transition-all group-hover:translate-x-1 group-hover:opacity-100" />
        </button>
        
        <button class="group flex h-16 w-full max-w-xs items-center justify-center gap-3 rounded-2xl border border-white/10 bg-white/5 px-8 text-lg font-bold text-white backdrop-blur-sm transition-all hover:scale-105 hover:bg-white/10 sm:w-auto">
          <Mic class="h-6 w-6 text-cyan-400" />
          <span>Real-time Voice</span>
        </button>
      </div>
    </div>
  </section>
</template>
