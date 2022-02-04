<template>
  <nav class="nav" aria-label="Main Menu">
    <div class="nav-logo">
      <!-- <img src="/img/doling-circle.png" alt="Doling Neighborhood Association" /> -->
      <nuxt-link to="/">
        <img src="/img/tree-graphic.png" alt="Drawing of tree with bench underneath" aria-labelledby="navTitle" />
      </nuxt-link>
      <nuxt-link tag="h1" class="nav-logo__text text-center h4" to="/" id="navTitle"
        >Doling Neighborhood Association</nuxt-link
      >
    </div>
    <ul class="nav-links">
      <li class="nav-link">
        <nuxt-link class="btn" to="/">Home</nuxt-link>
      </li>
      <li class="nav-link">
        <nuxt-link class="btn" to="/about">About</nuxt-link>
      </li>
      <li class="nav-link">
        <nuxt-link class="btn" to="/blog">History</nuxt-link>
      </li>
      <li class="nav-link nav-link--social">
        <a href="https://nextdoor.com/neighborhood/doling--springfield--mo/" rel="noreferrer noopener">
          <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 195 195">
            <title>Doling Neighborhood on Nextdoor</title>
            <g data-name="Layer 2">
              <path
                d="M4 92a94 94 0 0 1 160-61A94 94 0 1 1 4 92Zm131-33a28 28 0 0 0-3-2c-21-13-53-7-67 15-2 3-6 3-8 0-4-4-3-10-4-15 0-2 0-3-3-3l-24 2c0 20 7 36 28 40 3 1 4 3 4 5v43c0 4 0 5 4 5h18c4 0 5-1 5-5V99a24 24 0 0 1 5-16c14-17 40-4 38 16v45c1 4 1 5 5 5h19c2 0 3-1 3-4V92c0-14-9-26-20-33Z"
                style="stroke-miterlimit: 10; stroke-width: 8px"
                data-name="Layer 1"
              />
            </g>
          </svg>
        </a>
        <a href="https://www.facebook.com/groups/1045034285583613/" rel="noreferrer noopener">
          <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 195 195">
            <title>Doling Neighborhood Association on Facebook</title>
            <g data-name="Layer 2">
              <path
                d="M192 98c0-52-43-94-94-94a95 95 0 0 0-15 187v-66H59V98h24V77c0-23 14-37 35-37a144 144 0 0 1 21 2v24h-11c-12 0-16 7-16 14v18h26l-4 27h-22v67a94 94 0 0 0 80-94Z"
                style="stroke-miterlimit: 10; stroke-width: 8px"
                data-name="Layer 1"
              />
            </g>
          </svg>
        </a>
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: 'Header',
  // mounted() {
  //   const nav = document.querySelector('nav')
  //   const supportPageOffset = window.pageXOffset !== undefined
  //   const isCSS1Compat = (document.compatMode || '') === 'CSS1Compat'

  //   let previousScrollPosition = 0

  //   const isScrollingDown = () => {
  //     let scrolledPosition = supportPageOffset
  //       ? window.pageYOffset
  //       : isCSS1Compat
  //       ? document.documentElement.scrollTop
  //       : document.body.scrollTop
  //     let isScrollDown

  //     if (scrolledPosition > previousScrollPosition) {
  //       isScrollDown = true
  //     } else {
  //       isScrollDown = false
  //     }
  //     previousScrollPosition = scrolledPosition
  //     return isScrollDown
  //   }

  //   const handleNavScroll = () => {
  //     if (isScrollingDown() && !nav.contains(document.activeElement)) {
  //       nav.classList.add('scroll-down')
  //       nav.classList.remove('scroll-up')
  //     } else {
  //       nav.classList.add('scroll-up')
  //       nav.classList.remove('scroll-down')
  //     }
  //   }

  //   var throttleTimer

  //   const throttle = (callback, time) => {
  //     if (throttleTimer) return

  //     throttleTimer = true
  //     setTimeout(() => {
  //       callback()
  //       throttleTimer = false
  //     }, time)
  //   }

  //   const mediaQuery = window.matchMedia('(prefers-reduced-motion: reduce)')

  //   window.addEventListener('scroll', () => {
  //     if (mediaQuery && !mediaQuery.matches) {
  //       throttle(handleNavScroll, 250)
  //     }
  //   })
  // },
}
</script>
<style lang="scss" scoped>
  
</style>