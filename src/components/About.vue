<script setup>
</script>

<template>
  <section id="about" class="about__section">
          <h2 class="about__title">
              <span class=""> 01. </span>
              About Me
          </h2>
          <div class="about__container">
              <div class="about__content">
                  <div class="about__content--text">
                      <p>
                          Hello! My name is
                          <span class="highlight">Steven Woh</span>.
                          Driven by a thirst for knowledge and a passion for technology, I embarked on a journey of web development in 2021, which led me to the exciting world of
                          <span class="highlight">Web Development</span>.
                      </p>
                      <p>
                          As a developer, my primary focus is on
                          <span class="highlight"> creating accessible </span> and <span class="highlight">inclusive products that cater to diverse audiences</span>.
                      </p>
                      <p>Here are a few technologies I’ve been working with recently:</p>
                  </div>
                  <ul class="about__technologies">
                      <li>JavaScript</li>
                      <li>TypeScript</li>
                      <li>Vue</li>
                      <li>Node.js</li>
                      <li>TailwindCSS</li>
                      <li>React</li>
                      <li>Quasar</li>
                      <li>My SQL</li>
                  </ul>
              </div>
              <div class="about__image">
                  <img src="../assets/profile.jpeg" alt="profile" />
              </div>
          </div>
  </section>

</template>

<style scoped>
.about__section {
    height: 100vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
}

.about__section > * + * {
    margin-top: 2.5rem;
}

.about__title {
    display: flex;
    align-items: center;
    color: #ccd6f6;
    font-size: var(--text-xl);
    font-weight: 600;
}

.about__title > span {
    font-size: var(--text-base);
    color: var(--primary-green);
    padding-right: 1rem;
}

.about__container {
    display: flex;
    flex-direction: column;
    align-items: center;
}

.about__container > * + * {
    margin-top: 3rem;
}

.about__content {
    flex: 1;
    padding-right: 2.5rem;
}

.about__content > * + * {
    margin-top: 1.25rem;
}

.about__image {
    width: 18rem;
    height: 18rem;
    position: relative;
    border-radius: 0.5rem;
}

.about__image > img {
    position: absolute;
    z-index: 10;
    top: 0;
    left: 0;
    bottom: 0;
    right: 0;
    width: 100%;
    height: 100%;
    border-radius: 0.5rem;
}

.about__content--text {
    font-size: var(--text-lg)
}

.about__content--text > * + * {
    margin-top: 1rem;
}

.about__technologies {
    /* inherit: none; */
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    row-gap: 0.5rem;
    font-size: var(--text-sm);
    list-style-type: disc;
    list-style-position: inside;
}

.about__technologies > li::marker {
    color: var(--primary-green);
}

@media (min-width: 640px) {
    .about__title {
        font-size: var(--text-2xl)
    }

    .about__title > span {
        font-size: var(--text-lg)
    }
}

@media (min-width: 768px) {
    .about__title {
        font-size: var(--text-3xl)
    }

    .about__title > span {
        font-size: var(--text-xl)
    }

    .about__container {
        flex-direction: row;
        align-items: flex-start;
        justify-content: space-between;
    }

    .about__container > * + * {
        margin-top: 0;
        margin-left: 3rem;
    }
}
</style>
