<template>
  <div class="projects">
    <Card
      v-for="project in projects"
      v-bind:key="project.title"
      v-bind:project="project"
    />
  </div>
</template>

<script>
import Card from '~/components/Card.vue';

export default {
  components: {
    Card
  },
  props: {
    projects: Array
  }
};
</script>

<style scoped>
.projects {
  display: grid;
  /* grid-template-columns: repeat(auto-fill, minmax(350px, 1fr)); */
  grid-template-columns: repeat(auto-fill, minmax(360px, 1fr));
  grid-auto-rows: auto;
  grid-gap: 1rem;
}
</style>
