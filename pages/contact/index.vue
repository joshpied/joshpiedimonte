<template>
  <div class="container">
    <Nav/>
    <h1 class="page-title">Contact</h1>
    <div class="contact-container">
      <div class="contact-list">
        <figure class="contact-item">
          <img class="contact-icon" src="/images/mail.svg" alt="E-mail icon"/>
          <figcaption class="link-container"><a class="link" href="mailto:joshpied@gmail.com">joshpied@gmail.com</a></figcaption>
        </figure>
        <figure class="contact-item">
          <img class="contact-icon" src="/images/github.svg" alt="Github icon"/>
          <figcaption class="link-container"><a class="link" href="https://github.com/joshpied" target="_blank">GitHub</a></figcaption>
        </figure>
      </div>
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

<style scoped>
  .contact-container {
    margin-left: 40%;
  }

  .contact-list {
    display: flex;
    flex-direction: column;
    margin-top: 15px;
  }

  .contact-item {
    display: flex;
    flex-direction: row;
    align-items: center;
    margin-top: 15px;
  }

  .contact-icon {
    width: 40px;
    filter: invert(36%) sepia(48%) saturate(404%) hue-rotate(182deg) brightness(92%) contrast(82%);
  }

  .contact-item figcaption {
    margin-left: 1em;
  }

  @media only screen and (max-width: 768px) {
    .contact-container {
      margin-top: 5px;
      margin-left: 10%;
      margin-right: 10%;
    }
  }

  @media (prefers-color-scheme: dark) {
    .contact-icon {
      filter: invert(100%) sepia(2%) saturate(37%) hue-rotate(150deg) brightness(117%) contrast(84%);
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
    color: var(--accent);
    text-decoration: none;
  }

  .link::after {
    content: "";
    position: absolute;
  }

  .link-container .link::after {
    top: 98%;
    height: 2px;
    width: 0;
    left: 5%;
    background-color: var(--accent);
    transition: 0.5s ease all .3s;
  }

  .link-container:hover .link::after {
    width: 90%;
    transition: 0.3s ease all;
  }

</style>
