<template>
  <input type="range" :value="value" @input="e => $emit('input', e.target.value)" v-bind="$attrs" />
</template>

<script>
export default {
  props: {
    value: {
      type: String,
      default: ''
    }
  }
}
</script>
