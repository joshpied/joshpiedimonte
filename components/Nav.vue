<template>
  <nav>
    <div class="link-container">
      <nuxt-link to="/" class="link">
        <img class="link-icon" src="/images/icons/home.svg" alt="Home icon" />
        <span class="link-text">Home</span>
      </nuxt-link>
    </div>
    <div class="link-container">
      <nuxt-link to="/about" class="link">
        <img class="link-icon" src="/images/icons/user.svg" alt="About icon" />
        <span class="link-text">About</span>
      </nuxt-link>
    </div>
    <div class="link-container">
      <nuxt-link to="/contact" class="link">
        <img class="link-icon" src="/images/icons/inbox.svg" alt="Inbox icon" />
        <span class="link-text">Contact</span>
      </nuxt-link>
    </div>
    <div class="link-container">
      <nuxt-link to="/projects" class="link">
        <img
          class="link-icon"
          src="/images/icons/folder.svg"
          alt="Folder icon"
        />
        <span class="link-text">Projects</span>
      </nuxt-link>
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
  display: flex;
  align-items: stretch;
}

.link-icon {
  filter: invert(43%) sepia(14%) saturate(1946%) hue-rotate(147deg)
    brightness(95%) contrast(89%);
}

.link-text {
  margin-left: 4px;
}

@media (prefers-color-scheme: dark) {
  .link-icon {
    filter: invert(100%) sepia(2%) saturate(37%) hue-rotate(150deg)
      brightness(117%) contrast(84%);
  }
}

@media only screen and (max-width: 520px) {
  .link {
    flex-direction: column;
    align-items: center;
    font-size: 0.75em;
  }

  .link-text {
    margin-left: 0;
  }
}
</style>
