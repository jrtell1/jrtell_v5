<template>
  <div class="container mx-auto my-6 px-4">
    <div class="project">
      <div class="project__image">
        <img class="w-full" src="https://res.cloudinary.com/jrtell/image/upload/c_scale,f_auto,q_auto,w_300/v1565694490/jrtell/SharedScreenshot">
      </div>
      <div class="project__content">
        <h2 class="project__title">JRTell.se</h2>
        <p>
          Latest version of my personal site. I rebuild it from scratch every now and then as I get new ideas and become bored of the current design.
          Built with <a href="https://nuxtjs.org/" target="_blank" rel="noopener noreferrer">Nuxt.js</a> and <a href="https://tailwindcss.com/" target="_blank" rel="noopener noreferrer">tailwind.css</a>.
          Statically generated with Nuxt and hosted by <a href="https://www.netlify.com/" target="_blank" rel="noopener noreferrer">Netlify</a>.
        </p>
      </div>
    </div>

    <div class="project">
      <div class="project__image">
        <img class="w-full" src="https://res.cloudinary.com/jrtell/image/upload/c_scale,f_auto,q_auto,w_300,e_blur:200/v1552844646/jrtell/secret">
      </div>
      <div class="project__content">
        <h2 class="project__title">Secret Project - Work In Progress</h2>
        <p>
          A personal project I've been working on for almost a year. Soon ready for an initial release.<br>
          Built as a PWA (Progressive Web Application). A platform for direct trade between local producers and consumers in communities.
        </p>
      </div>
    </div>

    <div class="project">
      <div class="project__image">
        <img class="w-full" src="https://res.cloudinary.com/jrtell/image/upload/c_scale,f_auto,q_auto,w_300/v1552838252/jrtell/hemlagat">
      </div>
      <div class="project__content">
        <h2 class="project__title">Restaurang Hemlagat</h2>
        <p>
          My first jamstack!<br>
          The objective was to create a quick and simple website. I decided to use <a href="https://nuxtjs.org/" target="_blank" rel="noopener noreferrer">Nuxt.js</a> and its
          static site generator, combined with <a href="https://www.netlify.com/" target="_blank" rel="noopener noreferrer">Netlify</a> for hosting and deployment.<br>
          The lunch menu needed to be dynamically updated by non-technical users. I settled for <a href="https://www.contentful.com/" target="_blank" rel="noopener noreferrer">Contentful</a> as the headless CMS and backend for this.
        </p>
        <a class="button w-48" href="https://www.hemlagatjonkoping.se/" target="_blank" rel="noopener noreferrer">Check it out</a>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'index'
  };
</script>

<style lang="scss" scoped>
  .project {
    @apply flex flex-col items-center mb-32;
  }

  .project__image {
    @apply rounded-lg overflow-hidden h-40 w-64 shadow-lg flex-shrink-0;
  }

  .project__title {
    @apply text-4xl;
  }

  .project__content {
    @apply px-6;
  }

  @screen sm {
    .project {
      @apply flex-row;
    }
  }
</style>