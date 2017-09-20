<template>
  <bulma-hero :titulo="titulo" :subtitulo="subtitulo"></bulma-hero>
</template>

<script>
import BulmaHero from '../components/Hero'
export default {
  name: 'hello',
  components: {
    BulmaHero
  },
  data() {
    return {
      titulo: 'Vue.js pra quem nunca viu',
      subtitulo: 'Bulma.io',
    }
  }
}
</script>
