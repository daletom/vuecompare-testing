<template>
  <div>
    <h1>Compare Paint Changes to CC's Living Room</h1>
    <h2>Use the slider to reveal the before and after image.</h2>

    <VueCompareImage :style="{ maxWidth: '500px' }"
        leftImage="https://tom.imgix.net/cc/living1before.jpg?w=1000&h=1000&fit=crop&auto=format%2Ccompress"
        rightImage="https://tom.imgix.net/cc/living1after.jpg?w=1000&h=1000&fit=crop&auto=format%2Ccompress"
        alt="Living Room 1 image before and after"
        hover
    />

    <VueCompareImage :style="{ maxWidth: '500px' }"
        leftImage="https://tom.imgix.net/cc/living2before.jpg?w=1000&h=1000&fit=crop&auto=format%2Ccompress"
        rightImage="https://tom.imgix.net/cc/living2after.jpg?w=1000&h=1000&fit=crop&auto=format%2Ccompress"
        alt="Living Room 1 image before and after"
        hover
    />
  </div>
</template>

<script>
import VueCompareImage from 'vue-compare-image';

export default {
  components: { VueCompareImage },
  head() {
    return {
      title: 'The Dales',
      meta: [
        { name: 'twitter:title', content: 'The Dales' },
        { name: 'twitter:description', content: 'Dale Family Website' },
        {
          name: 'twitter:image',
          content: 'https://tom.imgix.net/thedales.svg?fm=png'
        },
        { name: 'twitter:card', content: 'summary_large_image' },
        { name: 'og:title', content: 'The Dales' },
        { name: 'og:type', content: 'website' },
        { name: 'og:url', content: 'https://thedales.me' },
        {
          name: 'og:image',
          content: 'https://tom.imgix.net/thedales.svg?fm=png'
        }
      ]
    }
  }
}
</script>
