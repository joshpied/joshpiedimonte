<template>
  <main>
    <h1 class="page-title">About</h1>
    <p class="about">
      Hi! My name's Josh and have been a web developer since 2017. Have a look
      around my projects and feel free to contact me for any requests or
      questions.
    </p>
  </main>
</template>

<style scoped>
p.about {
  margin-top: 15px;
  text-align: center;
  margin-left: 30%;
  margin-right: 30%;
  font-size: 24px;
  color: var(--accent);
  word-spacing: 5px;
  padding-bottom: 15px;
}

@media only screen and (max-width: 768px) {
  p.about {
    margin-top: 5px;
    margin-left: 5%;
    margin-right: 5%;
    font-size: 20px;
  }
}
</style>
