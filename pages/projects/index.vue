<template>
  <div class="container">
    <Nav />
    <h1 class="page-title">Projects</h1>
    <div class="projects">
      <Card
        v-for="project in projects"
        v-bind:key="project.title"
        v-bind:project="project"
      />
    </div>
  </div>
</template>

<script>
import Nav from '~/components/Nav.vue';
import Card from '~/components/Card.vue';

export default {
  components: {
    Nav,
    Card
  },
  data() {
    return {
      projects: [
        {
          title: 'Scape — Coming Soon!',
          description:
            'Scape is a sharing economy mobile application that directly connects customer to workers providing landscaping services. Scape was built using NativeScript/Angular and a Firebase backend',
          imageUrl: 'scape.jpg',
          route: 'projects/scape',
          type: 'internal'
        },
        {
          title: 'Coronavirus Projects',
          description:
            'Several dashboards and APIs made with React and Node.js, respectively, related to the COVID-19 outbreak',
          imageUrl: 'coronavirus-world-tracker.jpg',
          route: 'projects/coronavirus',
          type: 'internal'
        },
        {
          title: 'Calcio CLI',
          description:
            'Command line application to view the latest fixtures, standings, scores, and transfers in Serie A, built with Node',
          imageUrl: 'calcio.jpg',
          url: 'github.com/joshpied/calcio',
          type: 'external'
        },
        {
          title: 'QuickSnacks',
          description:
            'Digital recipe organizer built with React and Firebase. Uses a full WYSIWYG editor with user content being synced in real time',
          imageUrl: 'quicksnacks.jpg',
          url: 'quick-snacks.firebaseapp.com',
          type: 'external'
        },
        {
          title: 'MyHamiltonMap',
          description:
            'This app provides a comprehensive list of activities for visitors of Hamilton to build their own custom map of the city',
          imageUrl: 'my-hamilton-map.jpg',
          url: 'my-hamilton-maps.now.sh',
          type: 'external'
        },
        {
          title: 'Sampson Transmission',
          description:
            'Static site for Readers Choice Award winning auto repair shop Sampson Transmission',
          imageUrl: 'sampson-transmission.jpg',
          url: 'sampsontransmission.ca',
          type: 'external'
        },
        {
          title: 'Course & Grades',
          description:
            'Simple CRUD demo app app with filtering and sorting, built with Vue.js',
          imageUrl: 'courses-and-grades.jpg',
          url: 'courses-and-grades.now.sh',
          type: 'external'
        }
      ]
    };
  }
};
</script>

<style scoped>
.projects {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}
</style>
