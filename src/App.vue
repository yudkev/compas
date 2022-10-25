<script setup>
import { RouterLink, RouterView } from 'vue-router'

</script>

<template>
<main>
<header>
            <nav class="navbar level is-align-self-flex-end is-fixed-bottom">
              <p class="level-item has-text-centered">
               <RouterLink to="/"><a class="link is-info">Home</a></RouterLink>
              </p>
              <p class="level-item has-text-centered">
                <RouterLink to="/work"><a class="link is-info">Case Studies</a></RouterLink>
              </p>
              <p class="level-item has-text-centered is-hidden-mobile">
                <img src="../src/assets/ay3.png" alt="Alina Yudkevich" style="height: 65px">
              </p>
              <p class="level-item has-text-centered">
                 <RouterLink to="/cv"><a class="link is-info">CV</a></RouterLink>
              </p>
              <p class="level-item has-text-centered">
                <a class="link is-info" href="mailto:ayudkev@gmail.com">Contact</a>
              </p>
            </nav>
            </header>
            <section class="hero is-medium">
  <div class="hero-body">
    <p class="title">
      Alina Yudkevich
    </p>
    <p class="subtitle">
      Front-end developer and UX designer based in NYC.
    </p>
    <nav class="breadcrumb ml-0 is-size-7" aria-label="breadcrumbs">
      <ul>
        <li><a href="#">Github</a></li>
        <li><a href="#">Codepen</a></li>
        <li><a href="#">CV</a></li>
      </ul>
    </nav>
  </div>
</section>
</main>
            

  <RouterView />
</template>

<style scoped>
header {
  line-height: 1.5;
  max-height: 100vh;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
}
</style>
