<template>
  <footer>
    <ul class="footer-links">
      <li>Footer Link</li>
      <li>Footer Link</li>
    </ul>
  </footer>
</template>

<script>
export default {
  name: 'Footer',
}
</script>
<style lang="scss" scoped>
    footer {
        height: 200px;
        background-color: $green;
        flex-shrink: 0;
        margin-bottom: 0;
    }
    .footer-links {
        margin: 0;
    }
</style>