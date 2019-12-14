<template>
  <nav>
    <div class="link-container">
      <nuxt-link to="/" class="link">Home</nuxt-link>
    </div>
    <div class="link-container">
      <nuxt-link to="/about" class="link">About</nuxt-link>
    </div>
    <div class="link-container">
      <nuxt-link to="/contact" class="link">Contact</nuxt-link>
    </div>
    <div class="link-container">
      <nuxt-link to="/projects" class="link">Projects</nuxt-link>
    </div>
  </nav>
</template>

<style scoped>
  nav {
    display: flex;
    justify-content: flex-end;
  }

  @media only screen and (max-width: 768px) {
    nav {
      display: flex;
      justify-content: space-between;
    }
    .link-container {
      margin-left: 0 !important;
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
    color: var(--nav-link);
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
    background-color: var(--nav-link);
    transition: 0.5s ease all .3s;
  }

  .link-container:hover .link::after {
    width: 90%;
    transition: 0.3s ease all;
  }
</style>
