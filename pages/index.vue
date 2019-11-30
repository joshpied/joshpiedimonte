<template>
  <div class="container">
    <div>
      <h1 class="title">
        Josh Piedimonte
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
  import Logo from '~/components/Logo.vue'

  export default {
    components: {
      Logo
    }
  }
</script>

<style scoped>
  .container {
    margin: 0 auto;
    min-height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
  }

  .title {
    font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
    display: block;
    font-weight: 300;
    font-size: 100px;
    color: #35495e;
    letter-spacing: 1px;
  }

  .subtitle-container {
    text-align: left;
    display: flex;
    align-items: center;
    justify-content: space-between;
  }

  .subtitle {
    font-weight: 300;
    font-size: 42px;
    color: #526488;
    word-spacing: 5px;
    padding-bottom: 15px;
  }

  .link {
    position: relative;
    display: inline-block;
    font-size: 24px;
    font-weight: 400;
    text-align: center;
  }

  .link,
  .link:hover,
  .link:focus,
  .link:active {
    color: #526488;
    text-decoration: none;
  }

  .link::after {
    content: "";
    position: absolute;
  }

  .link-container .link::after {
    top: 98%;
    height: 2px;
    width: 0%;
    left: 5%;
    background-color: #526488;
    transition: 0.5s ease all .3s;
  }

  .link-container:hover .link::after {
    width: 90%;
    transition: 0.3s ease all;
  }
</style>
