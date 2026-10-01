<script setup>
import { projects } from '../data/projects'
</script>

<template>
  <header id="projects" class="hero">
    <div class="container">
      <h1>My Projects</h1>
      <p>Here are some of the projects I have worked on while learning web development.</p>
    </div>
  </header>

  <section class="projects-section">
    <div class="container">
      <div class="project-grid">
        <article v-for="project in projects" :key="project.slug" class="project-card">
          <img
            class="project-image"
            :src="project.image"
            :alt="project.name + ' project screenshot'"
            loading="lazy"
          >
          <div class="project-content">
            <p class="project-stage">{{ project.stage }}</p>
            <h2>{{ project.name }}</h2>
            <p>{{ project.description }}</p>

            <ul class="tags">
              <li v-for="technology in project.technologies" :key="technology">
                {{ technology }}
              </li>
            </ul>

            <div class="project-links">
              <a
                v-if="project.github"
                :href="project.github"
                target="_blank"
                rel="noopener noreferrer"
                class="project-link project-detail-link"
              >View on GitHub</a>
              <a
                v-if="project.live && project.live.length > 0"
                :href="project.live[0].url"
                target="_blank"
                rel="noopener noreferrer"
                class="project-link project-link-live"
              >View live project</a>
            </div>
          </div>
        </article>
      </div>
    </div>
  </section>
</template>
