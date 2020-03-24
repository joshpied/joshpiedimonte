<template>
  <div class="container">
    <Nav />
    <h1 class="page-title">Coronavirus Projects</h1>
    <div class="projects">
      <Card
        title="Coronavirus World Tracker"
        description="Dashboard built using Next.js and Charts.js. Displays worldwide COVID-19 statistics in addition to individual countries"
        imageUrl="coronavirus-world-tracker.jpg"
        url="coronavirus-world-tracker.now.sh"
      />
      <Card
        title="Coronavirus Italy Tracker"
        description="Dashboard tracking the most recent statistics specific to COVID-19 in Italy built with React, Mapbox, and Charts.js. Uses a Node API I built that pulls in regional data daily"
        imageUrl="coronavirus-italy-tracker.jpg"
        url="coronavirus-italy-tracker.now.sh"
      />
			<Card
        title="Coronavirus Italy API"
        description="Rest API built with Node, pulling data daily from the Italian government dataset"
        imageUrl="coronavirus-italia-api.jpg"
        url="coronavirus-italia-api.now.sh"
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
