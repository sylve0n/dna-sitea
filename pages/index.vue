<template>
  <main>
    <Hero />
    <section class="mt-8">
      <h3 class="text-primary-600 dark:text-primary-400 max-w-5xl mx-auto">Latest blog post</h3>
      <button class="btn">Button</button>
      <posts post-type="blog" :amount="1" />
    </section>
  </main>
</template>
<script>
export default {
  head() {
    return {
      script: [{ src: 'https://identity.netlify.com/v1/netlify-identity-widget.js' }],
    }
  },
}
</script>
<style lang="scss" scoped>
  
</style>