<template>
  <header class="hero">
      <div class="container">
        <h1>Contact ME</h1>
        <p class="hero-intro">
          I’m always open to new opportunities and collaborations. Whether you
          have a question, a project idea, or just want to say hello, feel free
          to reach out. I look forward to connecting with you!
        </p>
      </div>
    </header>

    <section class="container content-padding split-contact-container" aria-label="Contact Kanya">
      <div class="info-sidebar">
        <h2>Connect With Us</h2>
        <p class="sidebar-intro">
          Feel free to reach out directly through my professional channels or
          social networks:
        </p>

        <div class="info-links-list">
          <a
            href="https://mail.google.com/mail/?view=cm&fs=1&to=khanya.njenjemane06%40gmail.com"
            target="_blank"
            rel="noopener noreferrer"
            class="info-item info-link"
          >
            <span class="info-label">Email:</span>
            <span>khanya.njenjemane06@gmail.com</span>
          </a>

          <div class="info-item">
            <span class="info-label">GitHub:</span>
            <a
              href="https://github.com/Kanya233"
              target="_blank"
              rel="noopener noreferrer"
              class="info-link"
            >Kanya233</a>
          </div>

          <div class="info-item">
            <span class="info-label">LinkedIn:</span>
            <a
              href="https://www.linkedin.com/in/kanya-masinda-436799413/"
              target="_blank"
              rel="noopener noreferrer"
              class="info-link"
            >kanya masinda</a>
          </div>
        </div>
      </div>

      <div class="form-container">
        <h2>Send Me a Message</h2>

        <form
          action="https://formspree.io/f/xgobkygd"
          method="POST"
          class="contact-form"
        >
          <div class="form-group">
            <label for="name">Full Name</label>
            <input
              id="name"
              name="name"
              type="text"
              placeholder="Your Full Name"
              autocomplete="name"
              required
            >
          </div>

          <div class="form-group">
            <label for="email">Email Address</label>
            <input
              id="email"
              name="email"
              type="email"
              placeholder="username@example.com"
              autocomplete="email"
              required
            >
          </div>

          <div class="form-group">
            <label for="message">Message</label>
            <textarea
              id="message"
              name="message"
              rows="5"
              placeholder="How can I help you?"
              required
            ></textarea>
          </div>

          <button type="submit" class="submit-btn">Send Message</button>
        </form>
      </div>
  </section>
</template>
