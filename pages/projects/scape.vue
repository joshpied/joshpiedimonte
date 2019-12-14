<template>
  <div class="container">
    <Nav/>
    <h1 class="page-title">Scape</h1>
    <main class="articles">
      <article>
        <h2>Background</h2>
        <hr/>
        <p>
          The emergence of the sharing economy is of particular interest to me. It is seemingly at the centre of
          peer-to-peer based businesses.
        </p>
        <p>
          This booming sector is of course not possible without the digitalization of labour. With an increasing amount
          of companies leveraging the capabilities of the internet to interact with
          customers and workers, the labour itself has been reshaped.
        </p>
        <p>
          The platforms that exist on users phones have now become the go to destinations for people seeking goods and
          services. This notion of giving people what they want and when they want it is a pillar in guiding many up and
          coming companies.
        </p>
      </article>
      <article>
        <h2>What Scape Provides</h2>
        <hr/>
        <p>
          Scape provides a platform for customers to request a Scape (i.e. getting their grass cut or snow shovelled
          from their driveways) by connecting them directly to a landscaper.
        </p>
        <p>
          On the worker side can view open Scape requests closest to them. Once they accept a request the customer is
          notified in real time on the status of the job, from worker travel to when the task is complete.
        </p>
        <p>
          When the job is completed by the worker, they have the ability to upload images of the landscape and the
          customer will be charged with the credit card linked to their account.
        </p>
      </article>
    </main>
    <h2>Screenshots</h2>
    <div class="gallery">
      <figure>
        <img src="/images/scape/customer-searching.png" alt="Looking for a Scaper spinner">
        <figcaption>Customer sending a Scape request</figcaption>
      </figure>
      <figure>
        <img src="/images/scape/job-complete-comparison.png" alt="Job complete comparison">
        <figcaption>Customer and worker side receipts on two different devices</figcaption>
      </figure>
      <figure>
        <img src="/images/scape/worker-job-available.png" alt="Job available">
        <figcaption>Worker accepting job request</figcaption>
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

<style scoped>
  .container {
    margin-left: 5%;
    margin-right: 5%;
  }

  h2 {
    color: var(--primary);
    margin-top: 1em;
    margin-bottom: 1em;
  }

  hr {
    color: var(--primary);
    display: none;
  }

  .articles {
    display: flex;
    justify-content: space-between;
  }

  article:last-child {
    margin-left: 20px;
  }

  article p {
    font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
    margin-top: 1em;
    font-weight: 300;
    font-size: 1.5em;
    color: var(--accent);
    letter-spacing: 1px;
  }

  .gallery {
    display: flex;
    justify-content: space-around;
  }

  figure {
    text-align: center;
  }

  figcaption {
    color: var(--accent);
  }

  @media screen and (max-width: 990px) {
    .articles {
      flex-wrap: wrap;
    }

    article:last-child {
      margin-left: 0;
    }

    .gallery {
      flex-wrap: wrap;
    }
  }

  @media (prefers-color-scheme: dark) {
    hr {
      display: block;
    }
  }
</style>
