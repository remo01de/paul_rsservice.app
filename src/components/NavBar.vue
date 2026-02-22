<template>
  <nav class="fixed top-0 left-0 right-0 z-50 bg-deep-space/80 backdrop-blur-xl border-b border-white/10">
    <div class="max-w-7xl mx-auto px-6 py-4 flex items-center justify-between">
      <div class="flex items-center gap-2">
        <Bot class="w-6 h-6 text-cyber-green" />
        <span class="font-mono text-lg font-semibold">Paul</span>
      </div>
      
      <div class="hidden md:flex items-center gap-8">
        <a v-for="link in navLinks" :key="link.href" 
           :href="link.href" 
           class="text-sm text-gray-400 hover:text-white transition-colors font-mono">
          {{ link.label }}
        </a>
      </div>

      <div class="flex items-center gap-3">
        <span class="relative flex h-2 w-2">
          <span class="animate-ping absolute inline-flex h-full w-full rounded-full bg-cyber-green opacity-75"></span>
          <span class="relative inline-flex rounded-full h-2 w-2 bg-cyber-green"></span>
        </span>
        <span class="text-xs font-mono text-cyber-green">ONLINE</span>
      </div>
    </div>
  </nav>
</template>

<script setup>
import { Bot } from 'lucide-vue-next'

const navLinks = [
  { href: '#hero', label: 'Home' },
  { href: '#features', label: 'Features' },
  { href: '#techstack', label: 'Tech Stack' },
  { href: '#contact', label: 'Kontakt' },
]
</script>
