<template>
  <div class="container mx-auto px-4">
    <h2 class="text-3xl mt-8">Front-End</h2>
    <div>
      <div class="proficiencies__column">
        <h4 class="proficiencies__title">Languages</h4>
        <ul class="proficiencies__list">
          <li>HTML</li>
          <li>CSS</li>
          <li>SCSS</li>
          <li>JavaScript</li>
          <li>Typescript</li>
        </ul>
      </div>
      <div class="proficiencies__column">
        <h4 class="proficiencies__title">Frameworks</h4>
        <ul class="proficiencies__list">
          <li>VueJs</li>
          <li>NuxtJs</li>
          <li>Socket.io</li>
          <li>Tailwind.css</li>
          <li>Bulma</li>
          <li>AnimeJs</li>
        </ul>
      </div>
      <div class="proficiencies__column">
        <h4 class="proficiencies__title">Tools</h4>
        <ul class="proficiencies__list">
          <li>Webpack</li>
        </ul>
      </div>
    </div>

    <h2 class="text-3xl mt-8">Back-End</h2>
    <div>
      <div class="proficiencies__column">
        <h4 class="proficiencies__title">Languages</h4>
        <ul class="proficiencies__list">
          <li>PHP</li>
          <li>SQL</li>
          <li>NodeJs</li>
        </ul>
      </div>
      <div class="proficiencies__column">
        <h4 class="proficiencies__title">Frameworks</h4>
        <ul class="proficiencies__list">
          <li>Laravel/Lumen</li>
          <li>Socket.io</li>
          <li>SailsJs</li>
        </ul>
      </div>
      <div class="proficiencies__column">
        <h4 class="proficiencies__title">Tools</h4>
        <ul class="proficiencies__list">
          <li>Vagrant</li>
          <li>Composer</li>
        </ul>
      </div>
    </div>

    <h2 class="text-3xl mt-8">DevOps</h2>
    <div>
      <div class="proficiencies__column">
        <ul class="proficiencies__list">
          <li>Docker</li>
          <li>Netlify</li>
          <li>Git</li>
          <li>Nginx</li>
          <li>Ubuntu/Linux</li>
          <li>Cloudinary CDN</li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'proficiencies'
  };
</script>

<style scoped>
  .proficiencies__column {
    @apply flex-1;
  }

  .proficiencies__title {
    font-size: 18px;
    font-weight: 500;
  }

  .proficiencies__list {
    @apply flex p-0 flex-wrap;
  }

  .proficiencies__list li {
    list-style: none;
    padding: 2px 10px;

    @apply flex items-center;
  }

  .proficiencies__list li::before {
    border-radius: 3px;
    content: "";
    display: inline-block;
    height: 10px;
    width: 10px;
    margin-right: 5px;
    background: #1c5ca0;
  }
</style>