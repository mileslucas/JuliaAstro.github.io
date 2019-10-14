<template>
  <header class="hero">
    <img v-if="data.heroImage" :src="$withBase(data.heroImage)" :alt="data.heroAlt || 'hero'" />

    <h1 v-if="data.heroText !== null" id="main-title">{{ data.heroText || $title }}</h1>

    <p class="description">{{ data.tagline || $description }}</p>
  </header>
</template>

<script>
export default {
  name: "Hero",
  computed: {
    data() {
      return this.$page.frontmatter;
    }
  }
};
</script>

<style lang="stylus" scoped>
.hero {
  text-align: center;

  img {
    max-width: 100%;
    max-height: 280px;
    display: block;
    margin: 3rem auto 1.5rem;
  }

  h1 {
    font-size: 3rem;
  }

  h1, .description, .action {
    margin: 1.8rem auto;
  }

  .description {
    max-width: 35rem;
    font-size: 1.6rem;
    line-height: 1.3;
    color: lighten($textColor, 40%);
  }
}

@media (max-width: $MQMobileNarrow) {
  .hero {
    img {
      max-height: 210px;
      margin: 2rem auto 1.2rem;
    }

    h1 {
      font-size: 2rem;
    }

    h1, .description, .action {
      margin: 1.2rem auto;
    }

    .description {
      font-size: 1.2rem;
    }
  }
}
</style>