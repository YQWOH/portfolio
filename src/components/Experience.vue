<script setup>
</script>

<template>
  <section id="experience" class="experience__section">
      <h2 class="title">
          <span class="highlight"> 02. </span>Where I've Worked
      </h2>
      <div class="cards">
          <div>
              <h3>
                  <span>Web Developer</span>
                  <span>
                      @
                      <a class="link-underline" href="#"> Willowglen Sdn Bhd </a>
                  </span>
              </h3>
              <p>July 2022 - Present</p>
              <div>
                  <ul>
                      <li>Developing and maintaining web application using languages such as Typescript, Quasar & Vue Js for Front End, Express & Node Js for backend.</li>
                      <li>Creating and integrating web applications and features to improve user experience.</li>
                      <li>Collaborating with designers, content creators, and other developers to ensure website functionality and design align.</li>
                      <li>Writing well-designed, testable and efficient code.</li>
                  </ul>
              </div>
          </div>
          <div>
              <h3>
                  <span>SAP Executive</span>
                  <span >
                      @
                      <a class="link-underline" href="#"> Top Glove Sdn Bhd </a>
                  </span>
              </h3>
              <p>July 2019 - June 2022</p>
              <div>
                  <ul>
                      <li>Perform SAP configuration, check and upload master data, unit testing, System Integrating testing, conduct UAT with user</li>
                      <li>Support user on IT part, liaise with different IT team to ensure project can be deliver on time and fulfil with the requirement</li>
                      <li>Handle change request and enhancement for FI and CO module.</li>
                  </ul>
              </div>
          </div>
      </div>
  </section>

</template>

<style scoped>
.experience__section {
    height: 100vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    margin-top: 300px;
}

.experience__section > * + * {
    margin-top: 2.5rem;
}

.experience__section > .title {
    display: flex;
    align-items: center;
    color: #ccd6f6;
    font-size: var(--text-xl);
    font-weight: 600;
}

.experience__section > .title > span {
    /* text-base text-[var(--primary-green)] sm:text-lg md:text-xl pr-4 */
    font-size: var(--text-base);
    color: var(--primary-green);
    padding-right: 1rem;
}

.experience__section > .cards {
    display: grid;
    grid-template-columns: 1fr;
    row-gap: 4rem;
}

/* shadow-xl hover:shadow-2xl hover:scale-105 transition-all duration-150 ease-in-out  */
.experience__section > .cards > div {
    padding: 2.5rem 2.5rem 2rem;
    border: 1px solid #374151;
    cursor: pointer;
    border-radius: 0.25rem;
}

.experience__section > .cards > div > h3 {
    margin-bottom: 0.5rem;
    color: #ccd6f6;
    font-size: var(--text-lg);
    font-weight: 400;
}

.experience__section > .cards > div > h3 > span:nth-child(2) > a {
    color: var(--primary-green);
    text-decoration: none;
}

.experience__section > .cards > div > p {
    font-weight: 200;
}

.experience__section > .cards > div > div {
    margin-top: 1rem;
}

/* list-disc list-inside marker:text-[var(--primary-green)] space-y-4 */
.experience__section > .cards > div > div > ul {
    list-style: disc;
    list-style-position: inside;
}

.experience__section > .cards > div > div > ul > * + * {
    margin-top: 1rem;
}

.experience__section > .cards > div > div > ul > li::marker {
    color: var(--primary-green);
}

@media (min-width: 640px) {
    .experience__section > .title {
        font-size: var(--text-2xl)
    }

    .experience__section > .title > span {
        font-size: var(--text-lg)
    }
}

@media (min-width: 768px) {
    .experience__section > .title {
        font-size: var(--text-3xl)
    }

    .experience__section > .title > span {
        font-size: var(--text-xl)
    }
}

@media (min-width: 1024px) {
    .experience__section > .cards {
        grid-template-columns: 1fr 1fr;
        gap: 2.5rem;
    }
}
</style>
