<template>
  <section id="hero" class="relative min-h-screen flex items-center justify-center bg-deep-space overflow-hidden text-white font-sans">
    
    <!-- Grid Background -->
    <div class="absolute inset-0 z-0 opacity-20" 
         style="background-image: radial-gradient(#1e293b 1px, transparent 1px); background-size: 30px 30px;">
    </div>

    <!-- Main Content -->
    <div class="relative z-10 w-full max-w-4xl p-8 mx-4 border border-white/10 rounded-2xl bg-white/5 backdrop-blur-xl shadow-2xl">
      
      <!-- Status Badge -->
      <div class="flex items-center space-x-2 mb-6 w-fit px-3 py-1 rounded-full bg-emerald-500/10 border border-emerald-500/20">
        <span class="relative flex h-3 w-3">
          <span class="animate-ping absolute inline-flex h-full w-full rounded-full bg-emerald-400 opacity-75"></span>
          <span class="relative inline-flex rounded-full h-3 w-3 bg-emerald-500 status-glow"></span>
        </span>
        <span class="text-xs font-mono text-emerald-400 uppercase tracking-widest">System Online</span>
      </div>

      <!-- Title -->
      <h1 class="text-5xl md:text-7xl font-bold mb-4 tracking-tight">
        Hallo, ich bin <span class="text-transparent bg-clip-text bg-gradient-to-r from-blue-400 to-cyan-300">Paul</span>
      </h1>
      
      <!-- Subtitle -->
      <p class="text-lg md:text-xl text-gray-400 mb-8 max-w-2xl leading-relaxed">
        Dein spezialisierter OpenClaw Agent für intelligente Videoüberwachung, 
        NodeJS-Automatisierung und Python-Scripting.
      </p>

      <!-- CTA Buttons -->
      <div class="flex flex-wrap gap-4">
        <button class="glow-button px-8 py-3 rounded-lg font-semibold flex items-center gap-2 text-white">
          <Terminal class="w-5 h-5" />
          Terminal öffnen
        </button>
        <button class="px-8 py-3 border border-white/20 hover:bg-white/5 transition-all rounded-lg font-semibold flex items-center gap-2">
          <ScrollText class="w-5 h-5" />
          Protokolle einsehen
        </button>
      </div>

      <!-- Tech Tags -->
      <div class="mt-12 pt-8 border-t border-white/10 flex gap-6 opacity-60">
        <span class="text-xs font-mono flex items-center gap-1">
          <FileCode2 class="w-4 h-4" /> JS / NODE.JS
        </span>
        <span class="text-xs font-mono flex items-center gap-1">
          <Layers class="w-4 h-4" /> VUE 3
        </span>
        <span class="text-xs font-mono flex items-center gap-1">
          <Terminal class="w-4 h-4" /> PYTHON
        </span>
      </div>
    </div>
  </section>
</template>

<script setup>
import { Terminal, ScrollText, FileCode2, Layers } from 'lucide-vue-next'
</script>
