<script setup>
import { ref } from 'vue'

const isOpen = ref(false)
const links = [
  { label: 'Home', path: 'home' },
  { label: 'About', path: 'about' },
  { label: 'Skills', path: 'skills' },
  { label: 'Projects', path: 'projects' },
  { label: 'Contact', path: 'contact' }
]

function closeMenu() {
  isOpen.value = false
}
</script>

<template>
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark-green">
    <div class="container">
      <a class="navbar-brand" href="#/home" @click="closeMenu">MY PORTFOLIO</a>
      <button
        class="navbar-toggler"
        type="button"
        aria-controls="navbarNav"
        :aria-expanded="isOpen"
        aria-label="Toggle navigation"
        @click="isOpen = !isOpen"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div id="navbarNav" class="collapse navbar-collapse" :class="{ show: isOpen }">
        <ul class="navbar-nav ms-auto">
          <li v-for="link in links" :key="link.path" class="nav-item">
            <a
              class="nav-link"
              :class="{ active: link.path === 'home' }"
              :href="`#/${link.path}`"
              @click="closeMenu"
            >{{ link.label }}</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>
