<template>
  <div class="tricolor__block">
    <nuxt-link :to="{ link }">
      <h1 class="h4" v-if="title">{{ title }}</h1>
      <p v-if="subtitle">{{ subtitle }}</p>
    </nuxt-link>
  </div>
</template>

<script>
export default {
  name: 'TricolorBlock',
  props: {
    title: {
      type: String,
      default: '',
    },
    subtitle: {
      type: String,
      default: '',
    },
    link: {
      type: String,
      default: '',
    },
  },
}
</script>