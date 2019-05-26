<template>
  <div>
    <textarea v-model="matchText" />
  </div>
</template>

<script>
export default {
  props: {
    patternState: {
      type: Object,
      default: () => {}
    }
  },

  data: function () {
    return {
      matchText: 'Hello world!'
    }
  },

  watch: {
    'patternState.pattern': function (val) {
      this.updateMatches()
    },

    'matchText': function (val) {
      this.updateMatches()
    }
  },

  methods: {
    updateMatches: function () {
      console.log('updating matches')
    }
  }
}
</script>

<style>
</style>
