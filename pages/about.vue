<template>
  <main>
    <section class="w-full max-w-5xl mx-auto">
      <h1 class="title">{{ page.title }}</h1>
      <p class="">{{ page.intro }}</p>
    </section>
  </main>
</template>

<script>
export default {
  async asyncData({ $content }) {
    const page = await $content('site/about').fetch()

    console.log(page)

    return {
      page,
    }
  },
}
</script>
