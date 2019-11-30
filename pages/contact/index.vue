<template>
  <div class="container">
    <Nav/>
    <h1 class="page-title">Contact</h1>
    <div class="contact-list">
      <figure class="contact-item">
        <img src="/images/mail.png" alt="E-mail icon" width="50px"/>
        <figcaption class="link-container"><a class="link" href="mailto:joshpied@gmail.com">joshpied@gmail.com</a></figcaption>
      </figure>
      <figure class="contact-item">
        <img src="/images/github.png" alt="Github icon" width="50px"/>
        <figcaption class="link-container"><a class="link" href="https://github.com/joshpied" target="_blank">GitHub</a></figcaption>
      </figure>
    </div>
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

<style>
  .contact-list {
    display: flex;
    flex-direction: column;
    margin-top: 15px;
    margin-left: 45%;
    margin-right: 45%;
  }

  .contact-item {
    display: flex;
    flex-direction: row;
    text-align: center;
    align-items: center;
  }

  .contact-item figcaption {
    margin-left: 1em;
  }

  @media only screen and (max-width: 768px) {
    .contact-list {
      margin-top: 5px;
      margin-left: 10%;
      margin-right: 10%;
    }
  }

  .link-container {
    margin-left: 2em;
  }

  .link {
    position: relative;
    display: inline-block;
    font-size: 24px;
    font-weight: 400;
    text-align: center;
  }

  .link,
  .link:hover,
  .link:focus,
  .link:active {
    color: #526488;
    text-decoration: none;
  }

  .link::after {
    content: "";
    position: absolute;
  }

  .link-container .link::after {
    top: 98%;
    height: 2px;
    width: 0%;
    left: 5%;
    background-color: #526488;
    transition: 0.5s ease all .3s;
  }

  .link-container:hover .link::after {
    width: 90%;
    transition: 0.3s ease all;
  }

</style>
