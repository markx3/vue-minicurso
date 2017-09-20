<template>
  <div>
    <bulma-hero :titulo="titulo" :subtitulo="subtitulo"></bulma-hero>
      <form>
        <bulma-input label="Nome" placeholder="Nome da pessoa"></bulma-input>
        <bulma-input label="Idade"
                     placeholder="Idade da pessoa"
                     type="number"></bulma-input>
      </form>
  </div>
</template>

<script>
import BulmaHero from '../components/Hero'
import BulmaInput from '../components/Input'

export default {
  name: 'hello',
  components: {
    BulmaHero,
    BulmaInput
  },
  data() {
    return {
      titulo: 'Vue.js pra quem nunca viu',
      subtitulo: 'Bulma.io',
    }
  }
}
</script>
