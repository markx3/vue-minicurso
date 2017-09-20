<template>
  <div class="field">
    <label class="label">{{label}}</label>
    <div class="control">
      <input class="input" :value="value"
                           :type="type"
                           @input="$emit('input', $event.target.value)"
                           :placeholder="placeholder"
                           >
    </div>
  </div>
</template>

<script>
  export default {
    props: {
      label: String,
      placeholder: String,
      value: [String, Number],
      type: {
        type: String,
        default: 'text'
      }
    }
  }
</script>
