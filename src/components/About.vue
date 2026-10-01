<script setup>
const values = [
  ['Innovation', 'Always exploring new ideas and modern tools to stay ahead of the curve.'],
  ['Creativity', 'Designing custom user interfaces that are highly functional and beautiful.'],
  ['Community', 'Sharing tech knowledge and inspiring others to master design logic.']
]
</script>

<template>
  <header class="hero">
      <div class="container">
        <h1>About Me</h1>
        <p>Full Stack Web Development Trainee</p>
      </div>
    </header>

    <section class="container profile-section" aria-labelledby="about-heading">
      <div class="profile-img-block">
        <img
          class="profile-pic"
          src="https://i.ibb.co/gbVkPcZ0/IMG-2034.jpg"
          alt="Kanya Masinda"
        >
      </div>

      <div class="profile-text-block">
        <h2 id="about-heading">About Me</h2>
        <p class="lead-text">I'm Kanya, a full stack Web development trainee at Life Choices Academy in Cape Town.</p>
        <p>I started coding with zero experience. Now, I am building clean, modern websites with semantic structural coding tools.</p>
        <p>I'm still learning, still growing and that's my superpower. Every line of code and every bug teaches me how to build better.</p>

        <div class="goal-card">
          <p>“My goal: Become a junior developer and create tech that helps people in my community.”</p>
        </div>
      </div>
    </section>

    <section class="highlights-section" aria-labelledby="drives-heading">
      <div class="container text-center-align">
        <h2 id="drives-heading" class="section-heading">What Drives Me</h2>
        <div class="cards-grid">
          <article v-for="value in values" :key="value[0]" class="custom-card-about">
            <h3 class="card-title-about">{{ value[0] }}</h3>
            <p class="card-text-about">{{ value[1] }}</p>
          </article>
        </div>
      </div>
  </section>
</template>
