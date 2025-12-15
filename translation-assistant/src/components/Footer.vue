<script setup lang="ts">
import { Globe } from 'lucide-vue-next';
</script>

<template>
  <footer class="border-t border-white/10 bg-slate-950 py-12">
    <div class="container mx-auto px-4">
      <div class="grid gap-8 md:grid-cols-4">
        <div class="md:col-span-2">
          <div class="flex items-center gap-2">
            <div class="flex h-8 w-8 items-center justify-center rounded-lg bg-cyan-500/20 text-cyan-400">
              <Globe class="h-5 w-5" />
            </div>
            <span class="text-lg font-bold text-white">Translation Assistant</span>
          </div>
          <p class="mt-4 max-w-xs text-sm text-slate-400">
            Empowering global communication with AI-driven precision and security.
          </p>
        </div>
        
        <div>
          <h4 class="mb-4 text-sm font-semibold text-white">Product</h4>
          <ul class="space-y-2 text-sm text-slate-400">
            <li><a href="#" class="hover:text-cyan-400">Document Translation</a></li>
            <li><a href="#" class="hover:text-cyan-400">Real-time Voice</a></li>
            <li><a href="#" class="hover:text-cyan-400">OCR Engine</a></li>
            <li><a href="#" class="hover:text-cyan-400">Security</a></li>
          </ul>
        </div>
        
        <div>
          <h4 class="mb-4 text-sm font-semibold text-white">Company</h4>
          <ul class="space-y-2 text-sm text-slate-400">
            <li><a href="#" class="hover:text-cyan-400">About</a></li>
            <li><a href="#" class="hover:text-cyan-400">Blog</a></li>
            <li><a href="#" class="hover:text-cyan-400">Contact</a></li>
            <li><a href="#" class="hover:text-cyan-400">Privacy</a></li>
          </ul>
        </div>
      </div>
      
      <div class="mt-12 flex flex-col items-center justify-between border-t border-white/10 pt-8 text-xs text-slate-500 md:flex-row">
        <p>&copy; 2024 Translation Assistant. All rights reserved.</p>
        <div class="mt-4 flex gap-6 md:mt-0">
          <a href="#" class="hover:text-white">Terms</a>
          <a href="#" class="hover:text-white">Privacy</a>
          <a href="#" class="hover:text-white">Cookies</a>
        </div>
      </div>
    </div>
  </footer>
</template>
