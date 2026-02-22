<template>
  <div class="min-h-screen bg-deep-space text-white">
    <NavBar />
    <main>
      <HeroSection />
      <FeatureShowcase />
      <TechStack />
    </main>
    <FooterSection />
  </div>
</template>

<script setup>
import NavBar from './components/NavBar.vue'
import HeroSection from './components/HeroSection.vue'
import FeatureShowcase from './components/FeatureShowcase.vue'
import TechStack from './components/TechStack.vue'
import FooterSection from './components/FooterSection.vue'
</script>
