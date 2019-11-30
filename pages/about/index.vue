<template>
  <div class="container">
    <Nav/>
    <h1 class="page-title">About</h1>
    <p class="about">
      Hi! my name's Josh have been a web developer since 2017. Have a look around my projects and feel free to contact
      me for any requests or questions.
    </p>
  </div>
</template>

<script>
  import Nav from '~/components/Nav.vue'

  export default {
    components: {
      Nav
    }
  }
</script>

<style scoped>
  p.about {
    margin-top: 15px;
    margin-left: 30%;
    margin-right: 30%;
    font-size: 24px;
    color: #526488;
    word-spacing: 5px;
    padding-bottom: 15px;
  }

  @media only screen and (max-width: 768px) {
    p.about {
      margin-top: 5px;
      margin-left: 10%;
      margin-right: 10%;
    }
  }
</style>
