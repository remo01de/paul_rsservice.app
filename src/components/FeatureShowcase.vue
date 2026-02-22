<template>
  <section id="features" class="relative py-24 bg-deep-space text-white">
    <div class="max-w-6xl mx-auto px-6">
      
      <!-- Section Header -->
      <div class="text-center mb-16">
        <h2 class="text-3xl md:text-4xl font-bold mb-4">
          Meine <span class="text-transparent bg-clip-text bg-gradient-to-r from-blue-400 to-cyan-300">Fähigkeiten</span>
        </h2>
        <p class="text-gray-400 max-w-xl mx-auto">
          Spezialisiert auf Automatisierung, Videoüberwachung und intelligente Datenverarbeitung.
        </p>
      </div>

      <!-- Features Grid -->
      <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-6">
        <div v-for="feature in features" :key="feature.title"
             class="group p-6 rounded-xl border border-white/10 bg-white/5 hover:bg-white/10 transition-all hover:border-blue-500/30">
          <div class="w-12 h-12 rounded-lg bg-blue-500/10 flex items-center justify-center mb-4 group-hover:bg-blue-500/20 transition-colors">
            <component :is="feature.icon" class="w-6 h-6 text-blue-400" />
          </div>
          <h3 class="text-lg font-semibold mb-2">{{ feature.title }}</h3>
          <p class="text-sm text-gray-400">{{ feature.description }}</p>
        </div>
      </div>

    </div>
  </section>
</template>

<script setup>
import { Cpu, Video, Code2, Zap, Database, Shield } from 'lucide-vue-next'

const features = [
  {
    icon: Cpu,
    title: 'Echtzeit-Datenverarbeitung',
    description: 'Schnelle Analyse und Verarbeitung von Datenströmen in Echtzeit mit NodeJS und Python.'
  },
  {
    icon: Video,
    title: 'Videoüberwachungs-Integration',
    description: 'Schnittstellen zu Hikvision und anderen Überwachungsprotokollen für intelligente Analysen.'
  },
  {
    icon: Code2,
    title: 'Automatisierungsscripts',
    description: 'Massgeschneiderte Skripte für wiederkehrende Aufgaben und Workflow-Optimierung.'
  },
  {
    icon: Zap,
    title: 'Schnelle Reaktionszeit',
    description: 'Optimierte Performance durch asynchrone Verarbeitung und intelligentes Caching.'
  },
  {
    icon: Database,
    title: 'Datenbank-Management',
    description: 'Effiziente Verwaltung von MySQL, PostgreSQL und NoSQL-Datenbanken.'
  },
  {
    icon: Shield,
    title: 'Security-First',
    description: 'Sichere Verbindungen, verschlüsselte Kommunikation und Best-Practice-Security.'
  }
]
</script>
