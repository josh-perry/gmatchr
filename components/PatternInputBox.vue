<template>
  <div>
    <input
      v-model="patternState.pattern"
      type="text"
    >
  </div>
</template>

<script>
export default {
  props: {
    patternState: {
      type: Object,
      default: () => {}
    }
  }
}
</script>

<style>
</style>
