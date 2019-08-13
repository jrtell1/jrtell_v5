<template>
  <div class="container text-center">
    <h2 class="second-subtitle text-3xl" key="second-subtitle">
      I build websites and full-featured web applications.
    </h2>
    <div class="flex flex-wrap">
      <project-item title="Restaurang Hemlagat" description="Nuxt.js, Netlify" image-src="https://res.cloudinary.com/jrtell/image/upload/c_scale,f_auto,q_auto,w_300/v1552838252/jrtell/hemlagat"/>
      <project-item title="Secret Project" description="Work In Progress, Nuxt.js, Lumen" image-src="https://res.cloudinary.com/jrtell/image/upload/c_scale,f_auto,q_auto,w_300,e_blur:200/v1552844646/jrtell/secret"/>
    </div>
  </div>
</template>

<script>
import ProjectItem from '../components/project-item';
export default {
  components: { ProjectItem }
}
</script>

<style scoped>
/* Sample `apply` at-rules with Tailwind CSS
.container {
  @apply min-h-screen flex justify-center items-center text-center mx-auto;
}
*/

  .container {
    margin: 300px auto 0 auto;
  }

  .second-subtitle {
    font-weight: 300;
    color: #526488;
    word-spacing: 5px;
    padding-bottom: 15px;
  }
</style>
