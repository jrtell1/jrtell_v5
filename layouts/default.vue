<template>
  <div>
    <div class="header py-6 h-48" :class="$route.name">
      <transition-group tag="div" class="relative max-w-5xl mx-auto">
        <img
          class="portrait absolute rounded-full shadow-lg h-48"
          src="https://res.cloudinary.com/jrtell/image/upload/w_200,h_200,c_fill,g_face,f_auto/v1552242769/jrtell/Snapchat-1254887129"
          alt="Me"
          key="portrait"
        >
        <nuxt-link tag="h1" to="/" class="title absolute cursor-pointer" key="title">
          John-Robin Tell
        </nuxt-link>
        <h2 class="subtitle absolute" key="subtitle">
          Fullstack Developer
        </h2>
      </transition-group>
    </div>
    <nuxt />
  </div>
</template>

<style lang="scss">
  html {
    font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
      Roboto, 'Helvetica Neue', Arial, sans-serif;
    font-size: 16px;
    word-spacing: 1px;
    -ms-text-size-adjust: 100%;
    -webkit-text-size-adjust: 100%;
    -moz-osx-font-smoothing: grayscale;
    -webkit-font-smoothing: antialiased;
    box-sizing: border-box;
  }

  *,
  *:before,
  *:after {
    box-sizing: border-box;
    margin: 0;
  }

  .header {
    background: url('https://images.unsplash.com/photo-1464822759023-fed622ff2c3b?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=2100&q=80') no-repeat;
    background-position-y: center;
    background-size: cover;
    text-shadow: 0px 0px 11px #292929;
  }

  .portrait {
    border: 5px solid #fff;
    transition: all .2s ease-out;
  }

  .title {
    font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
    display: block;
    font-weight: 300;
    font-size: 90px;
    color: #fff;
    letter-spacing: 1px;
    transition: all .25s ease-out;
    white-space: nowrap;
  }

  .subtitle {
    font-weight: 300;
    color: #fff;
    word-spacing: 5px;
    padding-bottom: 15px;
    transition: all .25s ease-out;
    white-space: nowrap;
    @apply text-5xl;
  }

  .index {
    &.header {
      text-shadow: 0px 0px 0px #292929;
    }

    .portrait {
      left: 50%;
      transform: translate(-50%, 90px);
    }

    .title {
      color: #35495e;
      left: 50%;
      font-size: 40px;
      transform: translate(-50%, 280px);
    }

    .subtitle {
      color: #526488;
      left: 50%;
      transform: translate(-50%, 260px);
      @apply text-3xl;
    }
  }

  @screen md {
    .index {
      &.header {
        text-shadow: 0px 0px 0px #292929;
      }

      .portrait {
        left: 50%;
        transform: translate(-50%, 90px);
      }

      .title {
        color: #35495e;
        left: 50%;
        transform: translate(-50%, 250px);
        font-size: 90px;
      }

      .subtitle {
        color: #526488;
        left: 50%;
        transform: translate(-50%, 290px);
        @apply text-5xl;
      }
    }
  }

  .portrait {
    top: -40px;
    left: -45px;
    transform: scale(0.45);
  }

  .title {
    top: -30px;
    left: -60px;
    transform: scale(0.45);
  }

  .subtitle {
    top: 35px;
    left: -5px;
    transform: scale(0.45);
  }

  @screen sm {
    .portrait {
      top: -40px;
      left: -30px;
      transform: scale(0.55);
    }

    .title {
      top: -30px;
      left: 0px;
      transform: scale(0.55);
    }

    .subtitle {
      top: 35px;
      left: 45px;
      transform: scale(0.55);
    }

  }

  .page-enter-active {
    transition: opacity 0.15s ease-out;
  }

  .page-leave-active {
    transition: opacity 0.15s ease-in;
  }

  .page-enter,
  .page-leave-active {
    opacity: 0;
  }
</style>
