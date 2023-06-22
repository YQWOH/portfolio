<script setup>
</script>

<template>
  <nav class="navigation__container">
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
  </nav>
</template>

<style scoped>
.navigation__container {
    display: none;
    align-items: center;
}

.navigation__links {
    display: flex;
    align-items: center;
    margin-right: 2.5rem;
}

.navigation__links > * + * {
    margin-left: 2.5rem;
}

/* Navigation Link */
.link__item {
    list-style: none;
}

.link__name {
    color: #ccd6f6;
    text-decoration: none;
}

.link__name:hover {
    color: var(--primary-green);
}

/* Mobile: Navigation */
.header--hidden {
    transform: translateY(-100%);
}

/* Media Queries */
@media (min-width: 768px) {
    .navigation__container {
        display: flex;
    }
}

@media (min-width: 768px) {
    .mobile__navigation {
        display: none;
    }
}
</style>
