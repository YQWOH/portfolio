<script setup>
import Home from './components/Home.vue';
import About from './components/About.vue';
import Navigation from './components/Navigation.vue';
import Experience from './components/Experience.vue';
import Work from './components/Work.vue';
import Contact from './components/Contact.vue';
import Foote from './components/Footer.vue';
</script>

<template>
 <header class="header">

  <div class="logo__container">
      <a href="/">
          <svg xmlns="http://www.w3.org/2000/svg" class="logo__image" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
              <path stroke-linecap="round" stroke-linejoin="round" d="M5.121 17.804A13.937 13.937 0 0112 16c2.5 0 4.847.655 6.879 1.804M15 10a3 3 0 11-6 0 3 3 0 016 0zm6 2a9 9 0 11-18 0 9 9 0 0118 0z" />
          </svg>
      </a>
  </div>
  <Navigation />
  <!-- <nav class="navigation__container">
      <ol class="navigation__links">
          <li class="link__item">
              <span class="highlight"> 01. </span>
              <a class="link__name underline" href="/#about"> About </a>
          </li>
          <li class="link__item">
              <span class="highlight">02.</span>
              <a class="link__name underline" href="/#experience"> Experience </a>
          </li>
          <li class="link__item">
              <span class="highlight">03.</span>
              <a class="link__name underline" href="/#work"> Work </a>
          </li>
          <li class="link__item">
              <span class="highlight">04.</span>
              <a class="link__name underline" href="/#contact"> Contact </a>
          </li>
      </ol>
  </nav> -->

    <!-- <button class="mobile__navigation">
        <svg class="menu__icon" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
            <path stroke-linecap="round" stroke-linejoin="round" d="M4 6h16M4 12h16m-7 6h7" />
        </svg>
    </button> -->
  </header>

  <main>
    <Home />
    <About />
    <Experience />
    <Work />
    <Contact />
  </main>
  <Foote />
</template>

<style scoped>
main {
  padding-left: 2rem;
  padding-right: 2rem;
}
.header {
    display: flex;
    padding: 2rem 2.5rem;
    position: sticky;
    top: 0;
    z-index: 50;
    background-color:  #0a192f;
    transition: transform 0.2s;
}

/* Logo */
.logo__container {
    flex: 1;
}

.logo__image {
    width: 3rem;
    height: 3rem;
    color: var(--primary-green);
}

.mobile__navigation {
    cursor: pointer;
    background-color: transparent;
    border: none;
}

.menu__icon {
    width: 2.5rem;
    height: 2.5rem;
    color: var(--primary-green);
}

</style>
