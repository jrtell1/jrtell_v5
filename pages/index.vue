<template>
  <div class="container">
    <div>
      <div class="flex flex-col items-center">
        <img class="rounded-full shadow-lg" src="https://res.cloudinary.com/jrtell/image/upload/w_200,h_200,c_fill,g_face,f_auto/v1552242769/jrtell/Snapchat-1254887129" alt="Me">
        <h1 class="title">
          John-Robin Tell
        </h1>
        <h2 class="subtitle text-5xl">
          Fullstack Developer
        </h2>
        <h2 class="subtitle text-3xl">
          I build websites and entire web applications.
        </h2>
      </div>
      <div class="flex">
        <project-item title="Restaurang Hemlagat" description="Nuxt.js, Netlify" image-src="https://res.cloudinary.com/jrtell/image/upload/c_scale,f_auto,q_auto,w_300/v1552838252/jrtell/hemlagat"/>
        <project-item title="Secret Project" description="Work In Progress, Nuxt.js, Lumen" image-src="https://res.cloudinary.com/jrtell/image/upload/c_scale,f_auto,q_auto,w_300,e_blur:200/v1552844646/jrtell/secret"/>
      </div>
    </div>
  </div>
</template>

<script>
import ProjectItem from '../components/project-item';
export default {
  components: { ProjectItem }
}
</script>

<style>
/* Sample `apply` at-rules with Tailwind CSS
.container {
  @apply min-h-screen flex justify-center items-center text-center mx-auto;
}
*/

.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
