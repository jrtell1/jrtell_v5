<template>
  <div class="navigation">
    <div class="flex max-w-4xl mx-auto">
      <nuxt-link to="/" class="link">Home</nuxt-link>
      <nuxt-link to="/projects" class="link">Projects</nuxt-link>
      <div class="spacer"></div>
      <nuxt-link to="/history" class="link">Work history</nuxt-link>
      <nuxt-link to="/contact" class="link">Contact</nuxt-link>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'navigation'
  };
</script>

<style scoped>
  .navigation {
    @apply bg-gray-200 fixed inset-x-0 bottom-0 z-10;
  }

  .spacer {
    @apply hidden;
  }

  @screen md {
    .navigation {
      @apply static;
    }

    .spacer {
      @apply block flex-1;
    }
  }

  .link {
    @apply flex-1 block p-4 flex items-center justify-center;
    transition: all .2s ease-out;
  }

  .link:hover {
    @apply underline bg-gray-300;
  }

  .nuxt-link-exact-active {
    @apply bg-gray-300;
  }
</style>