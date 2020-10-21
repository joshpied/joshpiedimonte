<template>
  <main class="bb-container">
    <header class="bb-header">
      <picture>
        <source srcset="/images/baker-buddy/logo.webp" type="image/webp" />
        <source srcset="/images/baker-buddy/logo.png" type="image/png" />
        <img
          src="/images/baker-buddy/logo.png"
          alt="Smiling slice of bread"
          style="width: 3em"
        />
      </picture>
      <h1 class="bb-h1">Baker Buddy</h1>
    </header>

    <section class="bb-section bb-features">
      <h2 class="bb-h2 bb-feature-title">How it Works</h2>
      <div class="bb-feature-left">
        <div class="bb-feature-description">
          <h3>Input your target weight</h3>
          <p>
            Determining measurements for the perfect loaf of bread is tedious.
            With Baker Buddy all you have to do is enter your target end weight
            and the baker percentages your ingredients.
          </p>
        </div>
        <picture class="bb-feature-image">
          <source
            srcset="/images/baker-buddy/add-mockup.webp"
            type="image/webp"
          />
          <source
            srcset="/images/baker-buddy/add-mockup.png"
            type="image/png"
          />
          <img
            src="/images/baker-buddy/add-mockup.png"
            alt="Add recipe screen"
            style="width: 15em"
          />
        </picture>
      </div>

      <div class="bb-feature-right">
        <div class="bb-feature-description">
          <h3>Baker Buddy does the calculations for you</h3>
          <p>
            Instead of manually calculating your ingredients based on the weight
            of the flour, the app takes care of everything for you. There's even
            a handy multiplier feature for when you need to scale up.
          </p>
        </div>
        <picture class="bb-feature-image">
          <source
            srcset="/images/baker-buddy/details-mockup.webp"
            type="image/webp"
          />
          <source
            srcset="/images/baker-buddy/details-mockup.png"
            type="image/png"
          />
          <img
            src="/images/baker-buddy/details-mockup.png"
            alt="Recipe details screen"
            style="width: 15em"
          />
        </picture>
      </div>

      <div class="bb-feature-left">
        <div class="bb-feature-description">
          <h3>View all of your favourite recipes</h3>
          <p>
            All of your recipes are stored in your phone for later editing and
            viewing.
          </p>
        </div>
        <picture class="bb-feature-image">
          <source
            srcset="/images/baker-buddy/list-mockup.webp"
            type="image/webp"
          />
          <source
            srcset="/images/baker-buddy/list-mockup.png"
            type="image/png"
          />
          <img
            src="/images/baker-buddy/list-mockup.png"
            alt="Recipe list screen"
            style="width: 15em"
          />
        </picture>
      </div>
    </section>

    <section class="bb-section bb-download">
      <h2 class="bb-h2">Get the App</h2>
      <p>Coming soon to the App Store and Google Play!</p>
    </section>

    <section class="bb-section bb-roadmap">
      <h2 class="bb-h2">Roadmap</h2>
      <ul>
        <li>Web App</li>
        <li>Sync across devices</li>
      </ul>
    </section>
  </main>
</template>

<style scoped>
.bb-header {
  margin-top: 40px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.bb-h1 {
  margin-left: 0.5em;
}

.bb-h2 {
  font-size: 3em;
  text-align: center;
  margin-bottom: 0.5em;
}

.bb-section {
  margin-top: 3em;
}

.bb-section:last-child {
  margin-bottom: 10em;
}

.bb-feature-title {
  grid-area: title;
}

.bb-feature-description {
  grid-area: description;
  place-self: center;
  margin-bottom: 10em;
}

.bb-feature-description h3 {
  margin-bottom: 1em;
}

.bb-feature-image {
  grid-area: image;
}

.bb-feature-left {
  display: grid;
  /* grid-template-columns: 1fr 1fr 1fr 1fr; */
  grid-template-columns: 1fr minmax(100px, 3fr) minmax(200px, 2fr) 1fr;
  grid-template-rows: auto;
  grid-template-areas:
    'title title title title'
    '. description image .';
  row-gap: 15px;
}

.bb-feature-right {
  display: grid;
  grid-template-columns: 1fr minmax(100px, 3fr) minmax(200px, 2fr) 1fr;
  grid-template-rows: auto;
  grid-template-areas:
    'title title title title'
    '. image description .';
  row-gap: 15px;
}

.bb-feature-top {
  display: grid;
  grid-template-columns: 1fr minmax(100px, 3fr) minmax(200px, 2fr) 1fr;
  grid-template-rows: auto;
  grid-template-areas:
    'title title title title'
    '. description description .'
    '. image image .';
  row-gap: 15px;
}

@media (max-width: 700px) {
  .bb-feature-description{
    margin-bottom: 1em;
  }
  .bb-feature-image {
    text-align: center;
  }

  .bb-feature-left,
  .bb-feature-right,
  .bb-feature-top {
    grid-template-columns: 1fr;
    grid-template-areas:
      'title'
      'description'
      'image';
  }
}

.bb-download {
  text-align: center;
}

.bb-roadmap {
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>
