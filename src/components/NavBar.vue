<template>
  <nav>
    <div class="logo">
      <svg viewBox="0 0 24 24" fill="white">
        <path d="M12 2L4 6v4c0 5.5 3.8 10.7 8 12 4.2-1.3 8-6.5 8-12V6l-8-4z"/>
        <circle cx="12" cy="12" r="3"/>
      </svg>
      <span>SkyPath</span>
    </div>
    <ul class="nav-links">
      <li><a href="#home">Home</a></li>
      <li><a href="#project">Project</a></li>
      <li><a href="#team">Team</a></li>
      <li><a href="#features">Features</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>
</template>

<script setup>
import { onMounted } from 'vue'

onMounted(() => {
  window.addEventListener('scroll', () => {
    const nav = document.querySelector('nav')
    if (window.scrollY > 100) {
      nav.style.background = 'rgba(0, 0, 0, 0.15)'
      nav.style.backdropFilter = 'blur(10px)'
      nav.style.boxShadow = '0 2px 10px rgba(255,255,255,0.15)'
    } else {
      nav.style.background = 'rgba(0, 0, 0, 0.15)'
      nav.style.backdropFilter = 'blur(8px)'
      nav.style.boxShadow = '0 2px 15px rgba(255,255,255,0.15)'
    }
  })
})
</script>