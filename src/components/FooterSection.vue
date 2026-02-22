<template>
  <footer id="contact" class="relative py-12 bg-deep-space border-t border-white/10 text-white">
    <div class="max-w-6xl mx-auto px-6">
      
      <div class="flex flex-col md:flex-row items-center justify-between gap-6">
        
        <!-- Logo -->
        <div class="flex items-center gap-2">
          <Bot class="w-6 h-6 text-cyber-green" />
          <span class="font-mono text-lg">Paul</span>
        </div>

        <!-- Status -->
        <div class="flex items-center gap-2 text-sm text-gray-400">
          <span class="relative flex h-2 w-2">
            <span class="animate-ping absolute inline-flex h-full w-full rounded-full bg-cyber-green opacity-75"></span>
            <span class="relative inline-flex rounded-full h-2 w-2 bg-cyber-green"></span>
          </span>
          <span class="font-mono">System Status: Operational</span>
        </div>

        <!-- Links -->
        <div class="flex items-center gap-4">
          <a href="https://github.com/openclaw" target="_blank" 
             class="p-2 rounded-lg hover:bg-white/10 transition-colors">
            <Github class="w-5 h-5 text-gray-400 hover:text-white" />
          </a>
          <a href="https://discord.com/invite/clawd" target="_blank"
             class="p-2 rounded-lg hover:bg-white/10 transition-colors">
            <MessageCircle class="w-5 h-5 text-gray-400 hover:text-white" />
          </a>
        </div>

      </div>

      <!-- Copyright -->
      <div class="mt-8 pt-8 border-t border-white/10 text-center text-xs text-gray-500 font-mono">
        © {{ currentYear }} Paul – OpenClaw Agent. Powered by Vue 3 + Tailwind CSS.
      </div>

    </div>
  </footer>
</template>

<script setup>
import { Bot, Github, MessageCircle } from 'lucide-vue-next'

const currentYear = new Date().getFullYear()
</script>
