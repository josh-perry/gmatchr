<template>
  <div>
    <textarea v-model="patternState.pattern" />
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
