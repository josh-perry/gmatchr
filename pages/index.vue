<template>
  <section class="container">
    <h1>gmatchr</h1>
    <h2>regexr but for Lua patterns!</h2>

    <PatternInputBox :pattern-state="state" />
    <TextOutputBox :pattern-state="state" />
  </section>
</template>

<script>
import PatternInputBox from '~/components/PatternInputBox.vue'
import TextOutputBox from '~/components/TextOutputBox.vue'

var state = {
  pattern: 'hello'
}

export default {
  components: {
    PatternInputBox,
    TextOutputBox
  },

  data () {
    return {
      state: state
    }
  }
}
</script>

<style>
</style>
