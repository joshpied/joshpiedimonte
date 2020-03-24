<template>
  <nuxt-link :to="route" class="card">
    <img
      :src="'/images/project-images/' + imageUrl"
      class="card-img"
      alt="My Hamilton Map web page"
      width="460"
      height="345"
    />
    <div class="card-text">
      <h4 class="card-text_title">{{ title }}</h4>
      <p class="card-text_description">
        {{ description }}
      </p>
    </div>
  </nuxt-link>
</template>

<script>
export default {
  props: ['title', 'description', 'imageUrl', 'route']
};
</script>

<style scoped>
.card {
  text-decoration: none;
  margin: 50px 40px 50px 40px;
  width: 450px;
  border-radius: 10px;
  background-color: rgba(250, 247, 248, 0.5);
  -webkit-box-shadow: 0 4px 6px -6px #222;
  -moz-box-shadow: 0 4px 6px -6px #222;
  box-shadow: 0 4px 6px -6px #222;
}

.card:hover {
  -webkit-box-shadow: 0 0 12px -5px #222;
  -moz-box-shadow: 0 0 12px -5px #222;
  box-shadow: 0 0 12px -5px #222;
  opacity: 0.8;
}

.card-img {
  border-radius: 10px 10px 0 0;
  width: 100%;
  height: auto;
}

.card-text {
  padding-bottom: 30px;
  margin: 10px;
}

.card-text_title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  color: var(--primary);
  text-decoration: none;
  letter-spacing: 1px;
}

.card-text_description {
  margin-top: 5px;
  color: var(--accent);
  word-spacing: 2px;
  padding-bottom: 15px;
}

@media (prefers-color-scheme: dark) {
  .card {
    background-color: rgba(250, 247, 248, 0.1);
  }
}
</style>
