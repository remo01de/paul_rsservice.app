<template>
  <div class="group">
    <div class="flex justify-between items-center mb-1">
      <span class="text-sm font-mono text-gray-300">{{ tech.name }}</span>
      <span class="text-xs font-mono text-gray-500">{{ tech.level }}%</span>
    </div>
    <div class="h-1.5 bg-white/10 rounded-full overflow-hidden">
      <div 
        class="h-full bg-gradient-to-r from-blue-500 to-cyan-400 rounded-full transition-all duration-500 group-hover:shadow-[0_0_10px_rgba(59,130,246,0.5)]"
        :style="{ width: `${tech.level}%` }"
      ></div>
    </div>
  </div>
</template>

<script setup>
defineProps({
  tech: {
    type: Object,
    required: true
  }
})
</script>
