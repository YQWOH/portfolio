<script setup>
</script>

<template>
 <section id="work" class="work__section">
      <h2 class="work__title">
          <span> 03. </span>
          Some Things I've Built
      </h2>
      <ul class="work__cards">
          <li class="work__card">
              <div class="project__container">
                  <p>Featured Project</p>
                  <h3 class="project__title">
                      <a href="#">Budget App</a>
                  </h3>
                  <div class="project__description">
                      <p>A budget application that can calculate the income and expense amount.</p>
                  </div>
                  <ul class="project__technologies">
                      <li>Vue Js</li>
                      <li>TailwindCSS</li>
                  </ul>
                  <div class="project__links">
                      <a class="z-10" target="_blank" href="https://master--friendly-meerkat-0fa5ac.netlify.app/">
                          website
                      </a>
                  </div>
              </div>
            
              <div class="project__image">
                  <img  src="../assets/budget.jpeg" alt="" />
              </div>
          </li>

          <li class="work__card">
              <div class="project__container">
                  <p>Featured Project</p>
                  <h3 class="project__title">
                      <a href="#">Weather Application</a>
                  </h3>
                  <div class="project__description">
                      <p>A weather application that able to show the selected city weather.</p>
                  </div>
                  <ul class="project__technologies">
                      <li>Vue Js</li>
                      <li>TailwindCSS</li>
                      <li>Pinia</li>
                  </ul>
                  <div class="project__links">
                      <a class="z-10" target="_blank" href="https://celadon-ganache-136900.netlify.app/">
                          website
                      </a>
                  </div>
              </div>

              <div class="project__image">
                  <img src="https://i0.wp.com/palawan-news.com/wp-content/uploads/2021/01/Weather-01.jpg?fit=496%2C331&ssl=1" alt="" />
              </div>
          </li>
      </ul>
  </section>

</template>

<style scoped>
.work__section {
    height: 100vh;
    display: flex;
    flex-direction: column;
    justify-content: start;
}

.work__section > * + * {
    margin-top: 2.5rem;
}

.work__title {
    display: flex;
    align-items: center;
    color: #ccd6f6;
    font-size: var(--text-xl);
    font-weight: 600;
}

.work__title > span {
    font-size: var(--text-base);
    color: var(--primary-green);
    padding-right: 1rem;
}

.work__cards {
    display: grid;
    grid-template-columns: 1fr;
    row-gap: 4rem;
}

.work__card {
    /* shadow-xl hover:shadow-2xl hover:scale-105 transition-all duration-150 ease-in-out */
    border-radius: 0.25rem;
    cursor: pointer;
    position: relative;
    list-style: none;
}

.project__container {
    padding: 2.5rem 2.5rem 2rem;
}

.project__container > p {
    color: var(--primary-green);
    font-size: var(--text-sm);
    margin: 0.625rem 0;
}

.project__title {
    /*  transition-all duration-150 */
    font-size: var(--text-xl);
    font-weight: 600;
    margin-bottom: 0.625rem;
}

.project__title > a {
    color: #ccd6f6;
    text-decoration: none;
}

.project__title::hover {
    color: var(--primary-green);
}

.project__description {
    padding: 1.25rem 0;
}

.project__technologies {
    display: flex;
    flex-wrap: wrap;
    margin: 0.625rem 0;
    font-size: var(--text-sm);
    font-weight: 300;
}

.project__technologies > li {
    margin: 0 0.625rem 0.25rem 0;
    list-style: none;
}

.project__links {
    display: flex;
    align-items: center;
    margin-top: 1.25rem;
}

.project__links > * + * {
    margin-left: 1rem;
}

.project__links > a {
    width: 1.25rem;
    height: 1.25rem;
    z-index: 10;
    color: #ccd6f6;
}

.project__links > a:hover {
    color: var(--primary-green);
}

.project__image {
    position: absolute;
    top: 0px;
    left: 0px;
    right: 0px;
    bottom: 0px;
    width: 100%;
    height: 100%;
    opacity: 10%;
}

.project__image > img {
    object-fit: cover;
    width: 100%;
    height: 100%;
}

@media (min-width: 640px) {
    .work__title {
        font-size: var(--text-2xl);
    }

    .work__title > span {
        font-size: var(--text-lg);
    }
}

@media (min-width: 768px) {
    .work__title {
        font-size: var(--text-3xl);
    }

    .work__title > span {
        font-size: var(--text-2xl);
    }
}

@media (min-width: 1024px) {
    .work__cards {
        grid-template-columns: 1fr 1fr;
        gap: 2.5rem;
    }
}
</style>
