<script setup>
</script>

<template>
  <section id="contact" class="contact__section">
      <h2 class="contact__title">
          <span> 04. </span>
          What's Next?
      </h2>
      <div class="contact__container">
          <div class="contact__content">
              <h3>Get In Touch</h3>
              <p>Although I’m not currently looking for any new opportunities, my inbox is always open. Whether you have a question or just want to say hi, I’ll try my best to get back to you!</p>
          </div>
          <div class="contact__cta">
              <a href="#"> Say Hello </a>
          </div>
      </div>
  </section>
</template>

<style scoped>
.contact__section {
    height: 100vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    padding-top: 40px;
}

.contact__section > * + * {
    margin-top: 2.5rem;
}

.contact__title {
    display: flex;
    align-items: center;
    color: #ccd6f6;
    font-size: var(--text-xl);
    font-weight: 600;
}

.contact__container > * + * {
    margin-top: 4rem;
}

.contact__content > * + * {
    margin-top: 1.5rem;
}

.contact__content > h3 {
    font-size: var(--text-4xl);
    font-weight: 600;
    color: #ccd6f6;
}

.contact__content > p {
    font-size: var(--text-lg)
}

.contact__title > span {
    font-size: var(--text-base);
    color: var(--primary-green);
    padding-right: 1rem;
}

.contact__cta > a {
    border: 1px solid var(--primary-green);
    color: var(--primary-green);
    border-radius: 0.25rem;
    padding: 1.25rem 1.75rem;
    text-decoration: none;
}

.contact__cta > a:hover {
    color: #0a192f;
    background-color: var(--primary-green);
    transition-property: all;
    transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);
    transition-duration: 150ms;
}

@media (min-width: 640px) {
    .contact__title {
        font-size: var(--text-2xl)
    }

    .contact__title > span {
        font-size: var(--text-lg)
    }

    .contact__content > h3 {
        font-size: var(--text-5xl)
    }
}

@media (min-width: 768px) {
    .contact__title {
        font-size: var(--text-3xl)
    }

    .contact__title > span {
        font-size: var(--text-xl)
    }

    .contact__content > h3 {
        font-size: var(--text-7xl)
    }
}
</style>
