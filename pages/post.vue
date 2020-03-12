<template>
  <div id="example">
    <p>Original message: "{{ message }}"</p>
    <p>Computed reversed message: "{{ reversedMessage }}"</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      message: 'helloworld wtf bbq sauce'
    }
  },
  computed: {
    reversedMessage: function() {
      var abc = 1
      abc = abc + 1

      return this.message
        .split('')
        .reverse()
        .join('')
    }
  }
}
</script>

<style scoped>
</style>