<template>
  <div>
    <h1 class="page-title">Projects</h1>
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
          title: 'Baker Buddy — Coming Soon!',
          description: `A baker's companion app built with React Native. Baker Buddy simplifies the process of manually calculating individual recipe measurements by taking the end dough weight and ingredient perctanges and the app handles the rest`,
          imageUrl: 'baker-buddy.jpg',
          route: 'baker-buddy.vercel.app',
          type: 'external'
        },
        {
          title: 'Scape',
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
          title: 'F1 CLI',
          description:
            'Command line application to view the latest standings and race results for the current Formula 1 season, written in Ruby',
          imageUrl: 'f1.jpg',
          url: 'github.com/joshpied/f1-cli',
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
          title: 'MyHamiltonMap',
          description:
            'This app provides a comprehensive list of activities for visitors of Hamilton to build their own custom map of the city',
          imageUrl: 'my-hamilton-map.jpg',
          url: 'my-hamilton-maps.now.sh',
          type: 'external'
        }
        // {
        //   title: 'Course & Grades',
        //   description:
        //     'Simple CRUD demo app app with filtering and sorting, built with Vue.js',
        //   imageUrl: 'courses-and-grades.jpg',
        //   url: 'courses-and-grades.now.sh',
        //   type: 'external'
        // }
      ]
    };
  }
};
</script>
