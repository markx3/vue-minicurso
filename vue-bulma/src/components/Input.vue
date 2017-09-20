<template>
  <div class="field">
    <label class="label">{{label}}</label>
    <div class="control">
      <input class="input" :type="type" :placeholder="placeholder">
    </div>
  </div>
</template>

<script>
  export default {
    props: {
      label: String,
      placeholder: String,
      type: {
        type: String,
        default: 'text'
      }
    }
  }
</script>
