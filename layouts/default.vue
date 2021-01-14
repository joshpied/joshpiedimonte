<template>
  <div class="container">
    <Nav />
    <nuxt />
  </div>
</template>

<script>
import Nav from '~/components/Nav.vue';

export default {
  components: {
    Nav
  }
};
</script>

<style>
html {
  background: var(--background);
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}

.container {
  margin: 2%;
}
</style>
