<script setup>
import { computed, onBeforeUnmount, onMounted, ref } from 'vue'
import Navbar from './components/Navbar.vue'
import Hero from './components/Hero.vue'
import About from './components/About.vue'
import Skills from './components/Skills.vue'
import Projects from './components/Projects.vue'
import Contact from './components/Contact.vue'
import Footer from './components/Footer.vue'

const currentHash = ref(window.location.hash)
const page = computed(() => {
  const requestedPage = currentHash.value.replace(/^#\/?/, '') || 'home'
  return ['home', 'about', 'skills', 'projects', 'contact'].includes(requestedPage) ? requestedPage : 'home'
})
const updatePage = () => { currentHash.value = window.location.hash }

onMounted(() => window.addEventListener('hashchange', updatePage))
onBeforeUnmount(() => window.removeEventListener('hashchange', updatePage))
</script>

<template>
  <Navbar />
  <main>
    <Hero v-if="page === 'home'" />
    <About v-else-if="page === 'about'" />
    <Skills v-else-if="page === 'skills'" />
    <Projects v-else-if="page === 'projects'" />
    <Contact v-else-if="page === 'contact'" />
  </main>
  <Footer />
</template>
