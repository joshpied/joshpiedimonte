<template>
  <div class="home-container">
    <div class="inner">
      <h1 class="title">
        Josh &nbsp; Piedimonte
      </h1>
      <div class="subtitle-container">
        <h2 class="subtitle">
          Web Developer
        </h2>
        <div class="link-container">
          <nuxt-link to="/about" class="link">About</nuxt-link>
        </div>
        <div class="link-container">
          <nuxt-link to="/contact" class="link">Contact</nuxt-link>
        </div>
        <div class="link-container">
          <nuxt-link to="/projects" class="link">Projects</nuxt-link>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue';

export default {
  layout: 'no_layout',
  components: {
    Logo
  }
};
</script>

<style scoped>
.home-container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.inner {
  padding: 0 10px 0 10px;
  box-shadow: 0px 0px 0px 5px #2c7d95;
  transition: box-shadow 0.6s linear;
  margin: 0.5em;
}

.inner:hover {
  box-shadow: 0px 0px 0px 10px #2c7d95;
}

.title {
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: var(--text);
  letter-spacing: 6px;
}

.subtitle-container {
  text-align: left;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.subtitle {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-weight: 300;
  font-size: 42px;
  color: var(--text);
  word-spacing: 5px;
  padding-bottom: 15px;
}

@media only screen and (max-width: 768px) {
  .home-container {
    min-height: 50vh;
    margin: 5%;
  }

  .inner {
    padding: 0;
    box-shadow: 0px 0px;
    transition: none;
    margin: 0;
  }

  .inner:hover {
    box-shadow: 0px 0px;
  }

  .title {
    font-size: 40px;
    margin-top: 30px;
  }

  .subtitle {
    font-size: 30px;
  }

  .subtitle-container {
    text-align: center;
    display: flex;
    flex-direction: column;
  }

  .link-container {
    margin-top: 40px;
    margin-left: 0;
  }
}
</style>
