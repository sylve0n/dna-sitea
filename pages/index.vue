<template>
  <main>
    <Hero :title="page.hero.title" :subtitle="page.hero.subtitle" :image="page.hero.heroImage" />
    <div class="tricolor">
      <div class="tricolor__block">
        <h1 class="p">Block One</h1>
      </div>
      <div class="tricolor__block">
        <h1 class="p">Block Two</h1>
      </div>
      <div class="tricolor__block">
        <h1 class="p">Block Three</h1>
      </div>
    </div>
    <div class="homepage-content">
      <p>
        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Debitis sapiente repudiandae cum magni accusantium
        mollitia aspernatur labore, non minus ab quas consequuntur sed dolor dignissimos neque atque perspiciatis
        tenetur quod?
      </p>
    </div>
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