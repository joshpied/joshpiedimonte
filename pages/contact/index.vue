<template>
  <main>
    <h1 class="page-title">Contact</h1>
    <div class="contact-container">
      <div class="contact-list">
        <figure class="contact-item">
          <img
            class="contact-icon"
            src="/images/icons/mail.svg"
            alt="E-mail icon"
          />
          <figcaption class="link-container">
            <a class="link" href="mailto:joshpied@gmail.com">Email</a>
          </figcaption>
        </figure>
        <figure class="contact-item">
          <img
            class="contact-icon"
            src="/images/icons/github.svg"
            alt="Github icon"
          />
          <figcaption class="link-container">
            <a class="link" href="https://github.com/joshpied" target="_blank"
              >GitHub
            </a>
          </figcaption>
        </figure>
      </div>
    </div>
  </main>
</template>

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
  filter: invert(43%) sepia(14%) saturate(1946%) hue-rotate(147deg)
    brightness(95%) contrast(89%);
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
    filter: invert(100%) sepia(2%) saturate(37%) hue-rotate(150deg)
      brightness(117%) contrast(84%);
  }
}

.link-container {
  margin-left: 2em;
}
</style>
