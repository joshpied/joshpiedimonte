<template>
  <div>
    <h1 class="page-title">Coronavirus Projects</h1>
    <CardGallery v-bind:projects="projects" />
  </div>
</template>

<script>
import CardGallery from '~/components/CardGallery.vue';

export default {
  components: {
    CardGallery
  },
  data() {
    return {
      projects: [
        {
          title: 'Coronavirus World Tracker',
          description:
            'Dashboard built using Next.js and Charts.js. Displays worldwide COVID-19 statistics in addition to individual countries',
          imageUrl: 'coronavirus-world-tracker.jpg',
          url: 'coronavirus-world-tracker.now.sh',
          type: 'external'
        },
        {
          title: 'Coronavirus Italy Tracker',
          description:
            'Dashboard tracking the most recent statistics specific to COVID-19 in Italy built with React, Mapbox, and Charts.js. Uses a Node API I built that pulls in regional data daily',
          imageUrl: 'coronavirus-italy-tracker.jpg',
          url: 'coronavirus-italy-tracker.now.sh',
          type: 'external'
        },
        {
          title: 'Coronavirus World API',
          description:
            'Rest API built with Node using Johns Hopkins CSSE dataset. Data formatted to get daily outbreak stats over time by country',
          imageUrl: 'coronavirus-world-api.jpg',
          url: 'coronavirus-world-api.now.sh/api',
          type: 'external'
        },
        {
          title: 'Coronavirus Italy API',
          description:
            'Rest API built with Node, pulling data daily from the Italian government dataset',
          imageUrl: 'coronavirus-italia-api.jpg',
          url: 'coronavirus-italia-api.now.sh',
          type: 'external'
        }
      ]
    };
  }
};
</script>
