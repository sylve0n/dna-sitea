<template>
  <section class="hero" style="background-image: url('https://images.unsplash.com/photo-1585938389612-a552a28d6914')">
    <h1 class="title text-center">Doling Neighborhood Association</h1>
    <h2 class="title text-center h3">Subtitle Text Aww Yeah</h2>
  </section>
</template>

<script>
export default {
  name: 'Hero',
}
</script>
<style lang="scss" scoped>
  .hero {
    padding: 1rem 2rem;
    display: flex;
    flex-direction: column;
    justify-content: center;
    background-size: cover;
    background-position: center;
    height: 250px;
    .title {
      margin-top: 0;
      margin-bottom: 0.5em;
    }
  }
</style>