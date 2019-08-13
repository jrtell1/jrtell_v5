<template>
  <div class="start-container">
    <div class="bg-gray-200 py-32">
      <div class="container mx-auto text-center flex justify-around items-center flex-col sm:flex-row">
        <div class="flex flex-col justify-center">
          <h2 class="second-subtitle text-3xl px-4">
            I build websites and fully-featured web applications.
          </h2>

          <div class="flex items-center justify-center">
            <nuxt-link class="button" to="/projects">Check out my latest projects</nuxt-link>
          </div>
        </div>

        <div class="w-64 h-64">
          <img src="/undraw_laravel_and_vue_59tp.svg" alt="Programmer illustration">
        </div>
      </div>
    </div>

    <div class="container py-32 mx-auto text-center flex justify-around items-center flex-col sm:flex-row">
      <div class="w-64 h-64">
        <img src="/undraw_work_time_lhoj.svg" alt="Programmer illustration">
      </div>
      <div class="py-4 px-4 flex flex-col items-center">
        <h2 class="second-subtitle text-4xl">Current occupation</h2>
        <div class="text-xl">Employed full-time and freelancing on the side</div>
        <a class="button" href="https://www.linkedin.com/in/john-robin-tell-b8bb235b/" target="_blank" rel="noopener noreferrer">LinkedIn</a>
      </div>
      <!--    <div class="flex flex-wrap">-->
      <!--      <project-item title="Restaurang Hemlagat" description="Nuxt.js, Netlify" image-src="https://res.cloudinary.com/jrtell/image/upload/c_scale,f_auto,q_auto,w_300/v1552838252/jrtell/hemlagat"/>-->
      <!--      <project-item title="Secret Project" description="Work In Progress, Nuxt.js, Lumen" image-src="https://res.cloudinary.com/jrtell/image/upload/c_scale,f_auto,q_auto,w_300,e_blur:200/v1552844646/jrtell/secret"/>-->
      <!--    </div>-->
    </div>
  </div>
</template>

<script>
import ProjectItem from '../components/project-item';
export default {
  components: { ProjectItem }
}
</script>

<style lang="scss" scoped>
  .start-container {
    margin: 250px auto 0 auto;
  }

  .second-subtitle {
    font-weight: 300;
    color: #526488;
    word-spacing: 5px;
  }
</style>
