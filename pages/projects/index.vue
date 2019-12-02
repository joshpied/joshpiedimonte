<template>
  <div class="container">
    <Nav/>
    <h1 class="page-title">Projects</h1>
    <div class="projects">
      <InternalCard title="Scape"
                    description="Scape is a sharing economy mobile application that directly connects customer to workers providing landscaping services. This was built using NativeScript/Angular"
                    imageUrl="scape.jpg"
                    route="projects/scape"
      />
      <Card title="MyHamiltonMap"
            description="This app provides a comprehensive list of activities for visitors of Hamilton to build their own custom map of the city."
            imageUrl="my-hamilton-map.jpg"
            url="my-hamilton-maps.now.sh"
      />
      <Card title="Course & Grades"
            description="Simple CRUD app app with filtering and sorting, built with Vue.js."
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
  }
</script>

<style>
  .container {
    margin: 20px;
  }

  .page-title {
    font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
    font-weight: 300;
    color: #35495e;
    letter-spacing: 1px;
    text-align: center;
    margin-top: 40px;
  }

  .projects {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
  }
</style>
