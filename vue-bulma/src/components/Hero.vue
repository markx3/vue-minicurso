<template>
  <section class="hero is-primary">
    <div class="hero-body">
      <div class="container">
        <h1 class="title">
          {{ titulo }}
        </h1>
        <h2 class="subtitle">
          {{ subtitulo }}
        </h2>
      </div>
    </div>
  </section>
</template>

<script>
  export default {
    props: {
      titulo: String,
      subtitulo: String,
    }
  }
</script>
