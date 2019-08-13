<template>
  <div class="container mx-auto my-6 px-4">
    <div class="employment">
      <h4>Alektum Group</h4>
      <div>2019 - Current</div>
      <div>Front-End Developer</div>
      <div>
        <a class="button w-48 my-0 py-2" href="https://www.alektumgroup.se/" target="_blank" rel="noopener noreferrer">Check it out</a>
      </div>
    </div>

    <div class="employment">
      <h4>Rebel Walls</h4>
      <div>2016 - 2019</div>
      <div>Systems Developer</div>
      <div>
        <a class="button w-48 my-0 py-2" href="https://rebelwalls.com/" target="_blank" rel="noopener noreferrer">Check it out</a>
      </div>
    </div>

    <div class="employment">
      <h4>Self-employed</h4>
      <div>2013 - 2016</div>
      <div>Fullstack Developer</div>
      <div></div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'history'
  };
</script>

<style scoped>
  .employment {
    display: flex;
    justify-content: space-between;
    transition: all 200ms ease-in-out;

    @apply p-4 my-4 bg-gray-200;
  }

  @media screen and (max-width: 600px) {
    .employment {
      display: block;
    }
  }

  .employment:hover {
    @apply shadow-lg;
  }
</style>