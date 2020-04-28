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
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
}

@media only screen and (max-width: 1281px) {
  .projects {
    justify-content: space-evenly;
  }
}
</style>
