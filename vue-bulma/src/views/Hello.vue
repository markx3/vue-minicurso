<template>
  <div>
    <bulma-hero :titulo="titulo" :subtitulo="subtitulo"></bulma-hero>
      <section calss="section">
        <form>
          <bulma-input label="Nome"
                       v-model="name"
                       placeholder="Nome da pessoa"></bulma-input>
          <bulma-input label="Idade"
                       v-model="age"
                       placeholder="Idade da pessoa"
                       type="number"></bulma-input>
          <bulma-button class="is-primary" @click="onClick()">
            Salvar
          </bulma-button>
        </form>
      </section>
  </div>
</template>

<script>
import BulmaHero from '../components/Hero'
import BulmaInput from '../components/Input'
import BulmaButton from '../components/Button'

export default {
  name: 'hello',
  components: {
    BulmaHero,
    BulmaInput,
    BulmaButton
  },
  data() {
    return {
      titulo: 'Vue.js pra quem nunca viu',
      subtitulo: 'Bulma.io',
      name: null,
      age: null
    }
  },
  methods: {
    onClick() {
      window.alert('ola')
      console.log('hello')
    }
  }
}
</script>
