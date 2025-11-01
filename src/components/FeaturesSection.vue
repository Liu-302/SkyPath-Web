<template>
  <section id="features" class="features">
    <h2>Features</h2>
    <div class="features-grid">
      <div class="feature-card" v-for="(item, index) in features" :key="index">
        <div class="feature-icon">
          <img :src="item.image" :alt="item.title" />
        </div>
        <h4>{{ item.title }}</h4>
      </div>
    </div>
  </section>
</template>

<script setup>
const features = [
  { title: 'Path Analysis', image: '../assets/path-analysis.png' },
  { title: 'Manual Adjustment', image: '../assets/manual-adjustment.png' },
  { title: 'Dynamic Simulation', image: '../assets/dynamic-simulation.png' },
  { title: 'Export Functionality', image: '../assets/export-functionality.png' }
]
</script>