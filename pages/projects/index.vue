<template>
  <div class="container">
    <Nav />
    <h1 class="page-title">Projects</h1>
    <div class="projects">
      <InternalCard
        title="Scape — Coming Soon!"
        description="Scape is a sharing economy mobile application that directly connects customer to workers providing landscaping services. Scape was built using NativeScript/Angular and a Firebase backend"
        imageUrl="scape.jpg"
        route="projects/scape"
      />
      <Card
        title="Coronavirus Italy Tracker"
        description="Dashboard tracking the most recent statistics relating to COVID-19 in Italy built with React, Mapbox, and Chart.js. Uses a Node API that I built that uses government posted data that updates daily"
        imageUrl="coronavirus-italy-tracker.jpg"
        url="coronavirus-italy-tracker.now.sh"
      />
      <Card
        title="Calcio CLI"
        description="Command line application to view the latest fixtures, standings, scores, and transfers in Serie A, built with Node"
        imageUrl="calcio.jpg"
        url="github.com/joshpied/calcio"
      />
      <Card
        title="QuickSnacks"
        description="Digital recipe organizer built with React and Firebase. Uses a full WYSIWYG editor with user content being synced in real time"
        imageUrl="quicksnacks.jpg"
        url="quick-snacks.firebaseapp.com"
      />
      <Card
        title="MyHamiltonMap"
        description="This app provides a comprehensive list of activities for visitors of Hamilton to build their own custom map of the city"
        imageUrl="my-hamilton-map.jpg"
        url="my-hamilton-maps.now.sh"
      />
      <Card
        title="Sampson Transmission"
        description="Static site for Readers Choice Award winning auto repair shop Sampson Transmission"
        imageUrl="sampson-transmission.jpg"
        url="sampsontransmission.ca"
      />
      <Card
        title="Course & Grades"
        description="Simple CRUD demo app app with filtering and sorting, built with Vue.js"
        imageUrl="courses-and-grades.jpg"
        url="courses-and-grades.now.sh"
      />
    </div>
  </div>
</template>

<script>
import Nav from '~/components/Nav.vue';
import Card from '~/components/Card.vue';
import InternalCard from '~/components/InternalCard.vue';

export default {
  components: {
    Nav,
    Card,
    InternalCard
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
