<template>
  <header id="skills" class="hero">
    <div class="container">
      <h1>My Tech Skills</h1>
      <p>The tools and languages I am mastering at Life Choices Academy</p>
    </div>
  </header>

  <main class="container content-padding">
    <section class="section-block" aria-labelledby="journey-heading">
      <h2 id="journey-heading" class="section-heading">My Learning Journey</h2>
      <div class="cards-grid">
        <article class="custom-card">
          <h3 class="card-title">Before Life Choices</h3>
          <p class="card-text">
            I had no coding background. I thought coding was only for geniuses, but I found out
            that you could do anything you put your mind into.
          </p>
        </article>

        <article class="custom-card">
          <h3 class="card-title">Week 1-4 at LC</h3>
          <p class="card-text">
            Learned Python, HTML structure, CSS styling, Flexbox, and an intro to JavaScript.
            Built my first webpage.
          </p>
        </article>

        <article class="custom-card">
          <h3 class="card-title">Now</h3>
          <p class="card-text">
            Learning JavaScript: functions, loops, and template literals. Built sum() and
            factorial() functions. This portfolio is my biggest project so far. The code is not
            perfect yet, but I'm focused on growth—every challenge teaches me something new and
            I'm improving daily.
          </p>
        </article>
      </div>
    </section>

    <section class="section-block skills-split" aria-label="Skills and current learning">
      <div class="table-container">
        <h2 class="section-heading">Skills</h2>
        <table class="custom-table">
          <thead>
            <tr>
              <th scope="col">Skill</th>
              <th scope="col">Level</th>
            </tr>
          </thead>
          <tbody>
            <tr><td>HTML</td><td>Beginner</td></tr>
            <tr><td>CSS</td><td>Beginner</td></tr>
            <tr><td>JavaScript</td><td>Beginner</td></tr>
            <tr><td>Git &amp; GitHub</td><td>Beginner</td></tr>
          </tbody>
        </table>
      </div>

      <div class="profile-text-block">
        <div class="goal-card learning-box">
          <h3>Currently Learning:</h3>
          <ul>
            <li>Responsive Design &amp; Flexbox</li>
            <li>JavaScript Functions &amp; Arrays</li>
            <li>Problem Solving with Code</li>
          </ul>
        </div>
      </div>
    </section>
  </main>
</template>
