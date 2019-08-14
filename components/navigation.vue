<template>
  <div class="navigation overflow-x-auto">
    <div class="flex max-w-4xl mx-auto">
      <nuxt-link to="/" class="link">Home</nuxt-link>
      <nuxt-link to="/projects" class="link">Projects</nuxt-link>
      <div class="spacer"></div>
      <nuxt-link to="/history" class="link">Work history</nuxt-link>
      <a href="https://github.com/jrtell1" class="link" target="_blank" rel="noopener noreferrer">GitHub</a>
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
    @apply bg-white border-t fixed inset-x-0 bottom-0 z-10;
  }

  .spacer {
    @apply hidden;
  }

  .nuxt-link-exact-active {
    @apply bg-gray-200;
  }

  @screen md {
    .navigation {
      @apply static bg-gray-200 border-0;
    }

    .nuxt-link-exact-active {
      @apply bg-gray-300;
    }

    .spacer {
      @apply block flex-1;
    }
  }

  .link {
    @apply flex-1 block p-4 flex items-center justify-center whitespace-no-wrap;
    transition: all .2s ease-out;
  }

  .link:hover {
    @apply underline bg-gray-300;
  }
</style>