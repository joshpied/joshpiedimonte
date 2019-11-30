<template>
  <div class="container">
    <Nav/>
    <h1 class="page-title">Scape</h1>
    <article>
      <h2>
        Project Background
      </h2>
      <p>
        The emergence of the sharing economy is of particular interest to me. It is seemingly at the centre of
        peer-to-peer based businesses.
      </p>
      <p>
        This booming sector is of course not possible without the digitalization of labour. The availability and
        prominence of internet technologies in the current age has ushered in a wave of success for peer-to-peer
        exchanges. With an increasing amount of companies leveraging the capabilities of the internet to interact with
        customers and workers, the labour itself has been reshaped.
      </p>
      <p>
        The platforms that exist on users phones have now become the go to destinations for people seeking goods and
        services. This notion of giving people what they want and when they want it is a pillar in guiding many up and
        coming companies.
      </p>
    </article>
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
  article {
    margin-left: 20%;
    margin-right: 20%;
  }

  article p {
    font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
    display: block;
    margin-top: 1em;
    font-weight: 300;
    font-size: 1.5em;
    color: #526488;
    letter-spacing: 1px;
  }
</style>
