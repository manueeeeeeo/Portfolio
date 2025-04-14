<template>
  <div class="min-h-screen bg-gradient-to-b from-gray-50 to-gray-200 text-gray-800 font-sans">
    <Header />
    <main class="p-6 max-w-5xl mx-auto animate-fade-in">
      <About />
      <Projects />
      <Skills />
      <Contact />
    </main>
    <Footer />
  </div>
</template>

<script setup>
import Header from './components/Header.vue'
import About from './components/About.vue'
import Projects from './components/Projects.vue'
import Skills from './components/Skills.vue'
import Contact from './components/Contact.vue'
import Footer from './components/Footer.vue'
</script>