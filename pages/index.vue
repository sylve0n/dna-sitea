<template>
  <main>
    <Hero :title="page.hero.title" :subtitle="page.hero.subtitle" :image="page.hero.heroImage" />
  </main>
</template>
<script>
import Hero from '~/components/Hero.vue'
export default {
  components: {
    Hero,
  },
  async asyncData({ $content }) {
    const page = await $content('site/home').fetch()
    return {
      page,
    }
  },
  head() {
    return {
      script: [{ src: 'https://identity.netlify.com/v1/netlify-identity-widget.js' }],
    }
  },
}
</script>
<style lang="scss" scoped>
  
</style>