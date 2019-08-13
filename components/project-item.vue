<template>
  <div class="project-item m-12">
    <div class="rounded-lg overflow-hidden h-40 w-64 shadow">
      <img class="w-full" :src="imageSrc">
    </div>
    <h2 class="text-xl">{{ title }}</h2>
    <div class="project-item__details">
      <div class="p-2">{{ description }}</div>
      <button class="w-full block bg-transparent hover:bg-blue-500 text-blue-700 font-semibold hover:text-white py-2 px-4 border border-blue-500 hover:border-transparent rounded">
        Read more
      </button>
    </div>
  </div>
</template>

<script>
  import anime from 'animejs';

  export default {
    name: 'project-item',

    props: ['title', 'imageSrc', 'description'],

    methods: {
      onHover() {
        anime({

        });
      }
    }
  };
</script>
